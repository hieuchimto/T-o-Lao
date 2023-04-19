# T-o-Lao
Đăng các code cần nhớ thông qua notion
#include <iostream>
#include <cstring>
using namespace std;

struct node
{
    string name;
    int marks;
    node *next;
};

node *make_node(string s, int n)
{
    node *new_node = new node();
    new_node->name += s;
    new_node->marks = n;
    new_node->next = NULL;
    return new_node;
}

// chen dau
void pushfront(node **head, string s, int n)
{
    node *new_node = make_node(s, n);
    if (*head == NULL)
    {
        *head = new_node;
        return;
    }
    new_node->next = *head;
    *head = new_node;
}
