There is a stored cross-site scripting attack in "Friendly Links" (column administrator rights)

![image-20231119212003542](./img/image1.png)



Click "Friendly Links" to add content![image-20231119210329264](./img/image2.png)

![image-20231119205057185](./img/image3.png)

You can see that the data is written to the database without filtering and escaping.Therefore, a stored XSS vulnerability exists.

![image-20231119205607457](./img/image4.png)

On the homepage of the website, the link content is output without escaping or filtering, and you can see that the javascript code is successfully executed.

![image-20231119211709601](./img/image5.png)

![image-20231119211808838](./img/image6.png)

