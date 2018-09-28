def find(l,e):
   if e in l:
      return l.index(e)
   else:
      return False

def test(l,e):
   r=find(l,e)
   if r!=False:
      print('{0} exists in {1}'.format(l[r],l))
   else:
      print('{0} not exists in {1}'.format(e,l))

test([1,2,3],5)
test([1,2,3],3)
test([1,2,3],1)


如果Python函数的参数是可变对象，传递的是引用，如果参数是不可变对象，传递的是值。
a=[]
b={}
for i in range(3):
   b['x']=i
   a.append(b)
print(a)


a[0]['x']=3
print(a)



改变一下位置，结果就不一样了



l=['a','b','c']
for x in l:
   l.remove(x)
print(l)
