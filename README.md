# Numpy_CheatSheet
Py file containing some useful numpy syntax for array operations
# Numpy Lib

# In[1]:


get_ipython().system('pip install numpy')


# In[2]:


import numpy as np


# # Array initialization

# In[3]:


a = np.array([3,5,6,7,8,9,10])
print(a)


# In[5]:


b = np.array([(1,2,3),(4,5,6),(7,8,9)])
print(b)


# 
# # Generating a Array

# In[6]:


c = np.arange(20)
print(c)


# In[8]:


d = np.linspace(1,10,5)
print(d)


# # Array Properties

# In[15]:


a = np.array([1,2,3,4,5,6])
print(a.ndim) #Array Dimension
print(a.itemsize) #Bit size of every element
print(a.dtype) #array Data type
print(a.size * a.itemsize) #memory occupied
print(a.size) # Size of the array


# In[4]:


b = np.array([(1,2,3),(4,5,6)])
#print(b)
b = b.reshape(3,2)
print(b)


# # Array Slicing

# In[9]:


b = np.array([(1,2,3),(4,5,6),(7,8,9)])
print(b[2,1])
print(b[0:,2])


# # Array Value Operations 

# In[11]:


c = np.array([(1,2,3),(4,5,6),(7,8,9)])
print(c.min())
print(c.max())
print(c.sum())


# # Array Arthmetic Operation

# In[12]:


e = np.array([1,2,3,4,5])
f = np.array([6,7,8,9,10])

print(e+f)
print(e-f)
print(e*f)
print(e/f)


# In[15]:


g = np.array([(1,2,3),(6,7,8)])
print(g.sum(axis=0))
print(np.sqrt(e))
print(np.log(e))
print(np.exp(e))
print(np.std(e))


# In[21]:


h = np.array([(3,4,5),(6,7,8)])
print(np.hstack((h,g)))
print(np.vstack((h,g)))
print(b.ravel())


# # END OF MODULE

# In[ ]:




