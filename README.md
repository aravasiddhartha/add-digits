class Solution(object):
    def addDigits(self, num):
        """
        :type num: int
        :rtype: int
        """
        while num >= 10:
            total = 0
            while num > 0:
                total += num % 10  # add last digit
                num //= 10         # remove last digit
            num = total
        return num
        
