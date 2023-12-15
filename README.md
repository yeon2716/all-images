# all-images
```
var imageUrls = [];
har.log.entries.forEach(function (entry) {
  if (entry.response.content.mimeType.indexOf("image/") !== 0) return;
  imageUrls.push(entry.request.url);
});
console.log(imageUrls.join('\n'));

```
# 이미지의 갯수가 작게 나오면 새로고침하면 이미지가 로드된다

![image](https://github.com/yeon2716/all-images/assets/145514579/af817fe6-1585-4459-8bea-081a095b14e6)


이미지 우클릭 - copy - copy all as HAR 
![image](https://github.com/yeon2716/all-images/assets/145514579/cd675cd5-f3d1-447c-8bc9-a898b969e74f)


# console창에 변수를 만든다

# var har = 위에 복사한 내용을 붙여넣는다  (그 값은 객채이다)

# 객채가 har이라는 변수에 할당되었고 그 아래에 download.js 안에 내용을 복사하여 console 붙여 넣으면 전체 이미지 주소가 일괄적으로 나타난다.



![image](https://github.com/yeon2716/all-images/assets/145514579/571942ab-680f-472e-b541-5cd50c016694)

