#https://daveceddia.com/react-redux-immutability-guide/#redux-update-an-object

Updating State in React
To apply these examples to plain React state, you just need to tweak a couple things in these examples.

Since React will shallow merge the object you pass into this.setState(), you don’t need to spread the existing state like you would with Redux.

In a Redux reducer, you might write this:

return {
  ...state,
  (updates here)
}
With plain React state, you can write it like this, without the spread operator:

this.setState({
  updates here
})