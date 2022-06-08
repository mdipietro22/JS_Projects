function palindrome(str) {
  let checkVal = /[\W_]/g;
  let regVal = str.toLowerCase().replace(checkVal, '');
  let reverseVal = regVal.split('').reverse().join('');
  return reverseVal === regVal;
  }

palindrome("eye");