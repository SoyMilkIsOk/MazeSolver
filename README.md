# MazeSolver
Python Maze Solver Project (CSPB 3104)

This is a maze solving project I made for my algorithms class last year in Python. To run the project on a custom maze a user can download any black and white maze image, save it to the directory with the Jupyter notebook and add a code block with the following: 

```python
img = cv2.imread('*YOUR_FILENAME*.JPG')
cv2.circle(img,(70,1750), 15, (255,0,0), -1) # add a circle centered at (600, 70) radius 10, color red (RGB: 255,0,0)
cv2.circle(img, (900,500), 15, (0,255,255), -1) # add a circle centered at (790,200) radius 10, color red (RGB: 255,0,0)
plt.imshow(img) # show the image on the screen 
plt.title('Amazing 3')
plt.show()
```

This first block of code allows the user to chose their start and ending points by drawing red and purple circles on the image.

```python
img = cv2.imread('*YOUR_FILENAME*.JPG') # read an image from a file using opencv (cv2) library
p = computeShortestPath(img, (70,1750), (900,500))
drawPath(img,p,10)
plt.imshow(img) # show the image on the screen 
plt.title('Amazing2 Solution')
plt.show()
```

This next block does the computation that solves the maze and also draws the solution on the picture using the "DrawPath" function.
