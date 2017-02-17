speed (100);
function spiral(N) {
  if (N > 0) {   // the recursive case.
  var len = spiral(N -1); // Assume we can do a smaller spiral.
  fd (10* N);  // Now draw just the last leg of the big spiral.
  rt(120); 
  return len + (10 * N);   // Return the whole length.
  } else {
  return 0;   // The base case is zero: zero length.
  }
}
pen(pink);
spiral(60);
