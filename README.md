# 876.-Middle-of-the-Linked-List
876. Middle of the Linked List
class Solution {
    public ListNode middleNode(ListNode head) {
        if (head == null || head.next == null) return head;
        if(head.next.next == null) return head.next;
        ListNode s = head;
        ListNode f = head;
        while(f != null && f.next != null)
        {
            s = s.next;
            f = f.next.next;
        }
        return s;
    }
    
}
