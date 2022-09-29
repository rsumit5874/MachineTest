# MachineTest
This project is made for educational purpose.


1. Reverse a String.
  void main() {
  String str= 'Sumit';
  String rev= str.split('').reversed.join();
  print(rev);
  
  //Output:- timuS
}

2. Reverse a String by using StringBuffer.
String reverseUsingStringBuffer(String input){
  var rev = StringBuffer();
  for(int i =input.length-1;i>=0;i--){
    rev.write(input[i]);
  }
  return rev.toString();
}

3. Reverse a String without using loop.
 void logicBloc(String? str)
 {
        if ((str==null)||(str.length <= 1))
        {
           print(str);
        }
        else
        {
            print(str[str.length-1]);
          
            logicBloc(str.substring(0,str.length-1));
        }
    }
 
 4. Remove duplicate element from element.
 void removeDuplicateElemet(String? str, List a)
 {
  print(str!.split('').toSet().toList().join());
  print(a.toSet().toList());
 }
 
 5. Remove duplicate elemet without using inbuild function.
List removeDuplicate(List a) {
    var result = [];
    int idx = 0;
    var tmp = [];

    for (int i = 0; i < a.length; i++) {
      if(!result.contains(a[i])){
        result.add(a[i]);
      }
    }
    return result;
}

6. Count duplicat element in array
 List<int> items = [1, 1, 1, 2, 3, 4, 5, 5];

  Map<int, int> count = {};
  items.forEach((i){
    count[i] = (count[i] ?? 0) + 1;
  });

  print(count.toString()); // {1: 3, 2: 1, 3: 1, 4: 1, 5: 2}

7. print Fibonacci Series.
  int n1=0,n2=1,n3;
  print(n1);
  print(n2);
  
  for(int i = 2 ;i <= 5; i++){
   n3 = n1+n2;
    print('$n3');
    n1 = n2;
    n2 = n3;
  }
  
 // Output: 0 1 1 2 3 5
                       
 8. Prime Numbers Up to 100.
   void primeNumberBetween(int start, int end){
            //loop through the numbers one by one
            for(int i=start; i < end; i++){
                bool isPrime = true;
                //check to see if the number is prime
                for(int j=2; j < i ; j++){
                if(i % j == 0){
                        isPrime = false;
                        break;
                      }
                }
                // print the number
                if(isPrime)
                {
                  print('$i');
                }
            }
}
      
                 
