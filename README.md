# solution
Solutions for python questions


Question1
Use python lists and make an list of numbers.
Write a function which returns sum of the list of numbers

sum=0
def  sum_list(a):
    global sum
    for a in list:
        sum = sum + a
    return sum

list=[34,78,45,90,23,6,7]
sum_list(list)
print(sum)
 
Question2 
Setup a dict structure like this in python
Dict1: (this is a key, value pair of user id and username)
{
   “1” : “name1”,
   “2” : “name2”,
   “3” : “name3”
} etc.. 
Dict2: (this is a key value pair of user id and exam score) 
{
   “1” : 50,
   “2” : 60
   “3” : 70
}
These are just sample data assume there are hundreds of users 

Write a function in python in python, which will return maximum i.e function should return dictionary like
{
  “3” : 70
}

dict={"1":40,"2":80,"3":160,"4":50,"5":30}
MaxValue = max(dict.items(),key=lambda  y : y[1])
print("{",MaxValue[0], ":" ,MaxValue[1],"}")
 
 
Question 3
Assume we have list like this
[0,0,0,1,1,1,0,0,0,1,1,0,1,1,1,1,0,0,1,1]
Basically a list of zero’s and one’s.
Write a python function to the number of maximum consecutive  one’s present in the array. 
g output for the above array would be 4

def max_occurance(list,x):
    count=0
    for i in list:
        if (i==x):
            count=count+1
    return count

list= [0,0,0,1,1,1,0,0,0,1,1,0,1,1,1,1,0,0,1,1]
x=max(lst,key=list.count)
print(x,"occurs ",max_occurance(list,x),"times")
 
 
Question 4
Design a mysql database. Requirements are as follows 


We have a user entity with columns username, password




Every use can have multiple addresses. Address entity will have column street, pincode, country, state, phone no. So one user can have multiple addresses. 


Design a db structure for this using create table sql syntax and submit that.
Next,
Write a route in flask or django GET, POST route to save a user, login a user, add/update address for that user.

 
Import .views *
Urlpatterns=[
    Path(‘login’,’views.login,name=’login’),
]
 
 
 
Views 
 
def login(request):
    Username=username.get()
    Password=password.get()
 
def  add2(request):
    add= userCreate()
    if request.method == 'POST':
        add = userCreate(request.POST, request.FILES)
        if add.is_valid():
            add.save()
            
        else:
            return HttpResponse( "Errors occured”)





