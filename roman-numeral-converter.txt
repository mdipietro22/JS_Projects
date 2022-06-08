function convertToRoman(num) {
 let lookup = {
   M:1000, CM:900, D:500, CD:400, C:100, XC:90, L:50, XL:40, X:10, IX:9, V:5, IV:4, I:1
 },
 romNum = '', i;
 for (i in lookup) {
   while (num >= lookup[i]) {
     romNum += i;
     num -= lookup[i];
   }
 }
 return romNum;
}

convertToRoman(36);