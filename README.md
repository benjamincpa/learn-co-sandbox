function removeFromCart(toBeRemoved) {
  var ifTrue = false;
  if (cart.length > 0){
 for (var i = 0; i < cart.length; i++){
  if (cart[i].hasOwnProperty(toBeRemoved)) {
    ifTrue = true;
    cart.splice(i, 1);
    
  } 
 }
}
 if (!ifTrue){
    console.log("That item is not in your cart.");
 }
  return cart;
 } 


removeFromCart('eggs');