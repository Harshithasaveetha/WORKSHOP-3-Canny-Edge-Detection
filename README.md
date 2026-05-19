# Canny Edge Detection using OpenCV

## Python Code

```python
import cv2
import matplotlib.pyplot as plt

img = cv2.imread('HARR.jpg', cv2.IMREAD_GRAYSCALE)

blurred = cv2.GaussianBlur(img, (5, 5), 0)

edges = cv2.Canny(blurred, 50, 150)

plt.figure(figsize=(10, 5))

plt.subplot(121)
plt.imshow(img, cmap='gray')
plt.title('Original Image')
plt.axis('off')

plt.subplot(122)
plt.imshow(edges, cmap='gray')
plt.title('Detected Edges')
plt.axis('off')

plt.show()
```
## Output
<img width="776" height="425" alt="download" src="https://github.com/user-attachments/assets/cfa61b05-cb42-439c-84b8-8fb7b05fd589" />

