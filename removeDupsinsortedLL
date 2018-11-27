/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode(int x) : val(x), next(NULL) {}
 * };
 */
class Solution {
public:
    ListNode* deleteDuplicates(ListNode* head) {
        ListNode* tempCur = new ListNode(0);
        ListNode* next = new ListNode(0);
        tempCur = head;
        while(tempCur != NULL){
            next = tempCur->next;
            if (next != NULL && tempCur->val == next->val){
                tempCur->next = next->next;
                delete next;
            }
            else{
                tempCur = next;
            }
        }
        return head;   
    }
};
