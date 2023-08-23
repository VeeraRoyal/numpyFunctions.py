# numpyFunctions.py
import numpy as np
class parentCls:
    array1 = np.array([[1, 3, 4, 5], [2, 3, 5, 6]])
    array2 = np.array([[2, 3, 4, 5], [2, 3, 5, 6]])
    array3 = np.array([[3, 4, 5, 6], [2, 3, 5, 6]])
    def myfunction1(self):
        print("default array1 details are :","\n",self.array1)
        # myarray=self.array1*2
        # print("myarray value is:",myarray)

    def myfunction2(self):
        print("default array1 details are :","\n",self.array2)
        # myarray1=self.array2+22
        # print("myarray1 value is:", myarray1)


    def myfunction3(self):
        print("default array1 details are :","\n", self.array3)
        # myarray2 = self.array2 / 22
        # print("myarray2 value is:", myarray2)

class childcls(parentCls):
    def myfunction4(self):
        array1=np.array([["banana","apple"],["dog","cat"]])
        print("after changes my array1 details:","\n",array1)
        print("default array2 value is:","\n",self.array2)
        print("default array3 value is:","\n",self.array3)

myobj=childcls()
myobj.myfunction1()
myobj.myfunction2()
myobj.myfunction3()
myobj.myfunction4()
