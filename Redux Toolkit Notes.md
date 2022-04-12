### Redux Toolkit

##### 1) Why Redux over Context API ?
i) When it comes to bigger applications, especially if they're built by a team of developers, One of the biggest challenges is state management.

ii) Yes, context API is very useful tool, but it clearly has its limits, especially when we talk about big applications with tons of features and that is why we use the most popular library called Redux.

iii) Well Redux is not part of official react even though they are used together.


##### 2) Why Redux ToolKit over Redux ?

i) Even though Redux solves a lot of problems, it also introduces some new headaches. In short, it requires bunch of annoying boilerplate and manual setup, especially when it comes to advanced features. Since you'll need to install more libraries and add some more config setup, which over time, especially if you have to do it for every project, just becomes annoying.

And this is where Redux Toolkit comes into play.......

##### 3) What Redux Toolkit is doing special ?

i) So creators of Redux notice the general need for opinionated approach while setting up Redux applications, and as a result, they came up with Redux Toolkit, which effectively is Redux with batteries.

ii) Basically, it means that all the popular extra libraries and setups are built in and do not require extra setup. As a result, there is no time consuming set up and over time it speeds up our workflow tremendously.

iii) So with Redux Toolkit, we get all of the benefits. 

### Store

Store is the entire state of our application

#### Setup Store

- create store.js

```js
import { configureStore } from '@reduxjs/toolkit';

export const store = configureStore({
  reducer: {},
});
```

##### In the above function we are passing object and in the object we are having reducer object and here we will set up our features. Just have a look that we are exporting store as Named export.

---

##### Now go to the index.js file and import store from the store.js file and import Provider from react-redux library (react-redux is a library that connects Redux to our application)

###### And similarly to context API, We want to wrap our entire application. So we're going to grab this provide .There's a store prop and we just want to pass in the store coming from the store.

- index.js

```js
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
import App from './App';
// import store and provider
import { store } from './store';
import { Provider } from 'react-redux';

ReactDOM.render(
  <React.StrictMode>
    <Provider store={store}>
      <App />
    </Provider>
  </React.StrictMode>,
  document.getElementById('root')
);
```

#### Setup Cart Slice

- application feature
- create features folder/cart
- create cartSlice.js

i) We import createSlice from reduxjs toolkit library

ii) We invoke that createSlice function and we want to give it a name(which can anything) and the second property as initialState where we just setup whatever state we want.

iii) If we log the cartSlice we would see like below on the console.(Logging before writing the export default cartSlice.reducer)

![image](https://user-images.githubusercontent.com/42731246/163037768-1a8cf819-c166-4534-a6a8-97db9653436c.png)

iv) And that is the reason we would write the export default cartSlice.reducer

v) So this reducer is the one that is going to control that state in this cartSlice And that's why we want to export what we want to export this and in the store we come with the key and say it as the reducer.

```js
import { createSlice } from '@reduxjs/toolkit';

const initialState = {
  cartItems: [],
  amount: 0,
  total: 0,
  isLoading: true,
};

const cartSlice = createSlice({
  name: 'cart',
  initialState,
});

console.log(cartSlice);

export default cartSlice.reducer;
```

iv) We are importing this above cartSlice function (as cartReducer naming convention) over inside the reducer object in store.js file (as key value pair, which is similar to combineReducers logic in earlier versions of redux)

v) the key we used as cart inside the reducer object is up to us and we can use any naming over here.

- store.js

```js
import { configureStore } from '@reduxjs/toolkit';
import cartReducer from './features/cart/cartSlice';

export const store = configureStore({
  reducer: {
    cart: cartReducer,
  },
});
```

#### Access store value

- create components/Navbar.js
- import useSelector hook from react-redux
- And the selector is looking for the function as a parameter and we get access to the entire state.

![image](https://user-images.githubusercontent.com/42731246/163040032-20aeed28-544e-4ae7-b611-d29b40fe2028.png)

```js
import { CartIcon } from '../icons';
import { useSelector } from 'react-redux';

const Navbar = () => {
  const { amount } = useSelector((state) => state.cart);

  return (
    <nav>
      <div className='nav-center'>
        <h3>redux toolkit</h3>
        <div className='nav-container'>
          <CartIcon />
          <div className='amount-container'>
            <p className='total-amount'>{amount}</p>
          </div>
        </div>
      </div>
    </nav>
  );
};
export default Navbar;
```

#### Setup Cart

- cartSlice.js
- cartItems is nothing but the data in the array format.

```js
import cartItems from '../../cartItems';

const initialState = {
  cartItems: cartItems,
  amount: 0,
  total: 0,
  isLoading: true,
};
```

- create CartContainer.js and CartItem.js
- CartContainer.js

```js
import React from 'react';
import CartItem from './CartItem';
import { useSelector } from 'react-redux';

const CartContainer = () => {
  const { cartItems, total, amount } = useSelector((state) => state.cart);

  if (amount < 1) {
    return (
      <section className='cart'>
        {/* cart header */}
        <header>
          <h2>your bag</h2>
          <h4 className='empty-cart'>is currently empty</h4>
        </header>
      </section>
    );
  }
  return (
    <section className='cart'>
      {/* cart header */}
      <header>
        <h2>your bag</h2>
      </header>
      {/* cart items */}
      <div>
        {cartItems.map((item) => {
          return <CartItem key={item.id} {...item} />;
        })}
      </div>
      {/* cart footer */}
      <footer>
        <hr />
        <div className='cart-total'>
          <h4>
            total <span>${total}</span>
          </h4>
        </div>
        <button className='btn clear-btn'>clear cart</button>
      </footer>
    </section>
  );
};

export default CartContainer;
```

- CartItems.js

```js
import React from 'react';
import { ChevronDown, ChevronUp } from '../icons';

const CartItem = ({ id, img, title, price, amount }) => {
  return (
    <article className='cart-item'>
      <img src={img} alt={title} />
      <div>
        <h4>{title}</h4>
        <h4 className='item-price'>${price}</h4>
        {/* remove button */}
        <button className='remove-btn'>remove</button>
      </div>
      <div>
        {/* increase amount */}
        <button className='amount-btn'>
          <ChevronUp />
        </button>
        {/* amount */}
        <p className='amount'>{amount}</p>
        {/* decrease amount */}
        <button className='amount-btn'>
          <ChevronDown />
        </button>
      </div>
    </article>
  );
};

export default CartItem;
```

#### First Reducer

- cartSlice.js
- Immer library

```js
const cartSlice = createSlice({
  name: 'cart',
  initialState,
  reducers: {
    clearCart: (state) => {
      state.cartItems = [];
    },
  },
});

export const { clearCart } = cartSlice.actions;
```

- create action

```js
const ACTION_TYPE = 'ACTION_TYPE';

const actionCreator = (payload) => {
  return { type: ACTION_TYPE, payload: payload };
};
```

- CartContainer.js

```js
import React from 'react';
import CartItem from './CartItem';
import { useDispatch, useSelector } from 'react-redux';

const CartContainer = () => {
  const dispatch = useDispatch();

  return (
    <button
      className='btn clear-btn'
      onClick={() => {
        dispatch(clearCart());
      }}
    >
      clear cart
    </button>
  );
};

export default CartContainer;
```
