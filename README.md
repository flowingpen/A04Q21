A04Q21
======
void move(struct node *head)
{
struct node *current=head,temp=current->next;
while(temp->next!=NULL)
{
temp=temp->next;
current=current->next;
}
current->next=NULL;
temp->next=head;
head=temp;
}
