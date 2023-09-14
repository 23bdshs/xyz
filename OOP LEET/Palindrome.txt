class Solution {
public:
    bool isPalindrome(int x) {
        string number = to_string(x) ;
        int length = number.size() ;
        for(int i = 0 ; i < length / 2 ; i ++){
            if(number[i] != number[length - i - 1])
                return false ;
        }
        return true;
    }
};