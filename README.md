# Program-to-count-the-number-of-nodes-(Transversing a single Linked List)

#include<stdio.h>
#include<stdlib.h>
struct node{
int data;
struct node *link;
};
int main(){
count_of_nodes(head);
}
void count_of_nodes(struct node *head)
{
int count=0;
if(head==NULL)
printf("Linked List is empty");
struct node *ptr=NULL;
ptr=head;
while(ptr!=NULL)
{
count++;
ptr=ptr->link;
}
printf("%d", count);
}
