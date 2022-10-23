#include <stdio.h> 
#include <stdlib.h> 
#define MAX 10

int count = 0; 

struct stack { 
    int items[MAX]; 
    int top; 
}; 

typedef struct stack st; 

void createstack(st*s){
    s->top = -1;
}

int isfull(st*s){
    if(s->top==MAX-1)
    return 1;
    else
    return 0;
}

int isempty(st*s){
    if (s->top==-1)
    return 1;
    else 
    return 0;
}

void push(st*s, int newitem){
    if (isfull(s)){
        printf("Stack is full");
    }
    else {
        s->top++;
        s->items[s->top] = newitem;
    }
    count++;
}

void pop(st*s){
    if(isempty(s)){
        printf("stack is empty");
    }
    else {
        printf("Removed item is: %d",s->items[s->top]);
        s->top--;
    }
    count--;
    printf("\n"); 
}

void display(st*s){
     printf("stack is:");
     for (int i=0;i<count;i++){
         printf("%d ",s->items[i]);
     }
    printf("\n"); 
}

int main()
{
    st*s=(st*)malloc(sizeof(st));
    createstack(s);
    push(s,98);
    push(s,25);
    push(s,34);  
    display(s);
    pop(s);
    display(s);
}
