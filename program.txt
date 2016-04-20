<<<<<<< HEAD
#include stdio.h
#include stdlib.h

int dynamicArray (int length) {
  int array;
  array = (int) malloc (length  sizeof(array));
  if (array == NULL) {
    return NULL;
  } else {
    int i;
    for (i = 0; i  length; i++){
      array[i] = 2  i + 1;
    }
    return array;
  }
}

int main (){
  int length;
  printf (Program creates an array of length given by You. Please give length );
  scanf (%d, &length);
  if (length  1) {
    printf (Invalid length. It has to be  0.);
  } else {
      int array;
      array = dynamicArray (length);
      if (array == NULL) {
            printf (nError during memory allocating.n);
      } else {
            int i;
            printf (Your arrayn);
            for (i = 0; i  length; i++){
              printf (%d , array[i]);
            }
            free(array);
      }
  }
    
  return 0;
=======
#include stdio.h
#include stdlib.h

int dynamicArray (int length) {
  int array;
  array = (int) malloc (length  sizeof(array));
  if (array == NULL) {
    return NULL;
  } else {
    int i;
    for (i = 0; i  length; i++){
      array[i] = 2  i + 1;
    }
    return array;
  }
}

int main (){
  int length;
  printf (Program creates an array of length given by You. Please give length );
  scanf (%d, &length);
  if (length  1) {
    printf (Invalid length. It has to be  0.);
  } else {
      int array;
      array = dynamicArray (length);
      if (array == NULL) {
            printf (nError during memory allocating.n);
      } else {
            int i;
            printf (Your arrayn);
            for (i = 0; i  length; i++){
              printf (%d , array[i]);
            }
            free(array);
      }
  }
    
  return 0;
>>>>>>> 0269eeab4d029bc975fc4ccab9f3844d8d5d06de
}