# S-Cart  
S-cart Link : https://s-cart.org/  
Gitbu Link : https://github.com/s-cart/s-cart     
# About S-Cart  
S-Cart is the best free e-commerce website project for individuals and businesses, built on top of Laravel Framework and the latest technologies. Our goal is "Efficient and friendly for everyone":  

- Efficiency: Meet even the smallest requirements of customers.  
- Friendly: Easy to use, easy to maintain, easy to develop.  
- Everyone: Businesses, individuals, developers, students.  

# Theme  
Theme Namr : E-Commerce  
Theme Auth : Maruf Ahmed  
Auth Email : biz.marufahmed@gmail.com  
Auth Website : http://maufahmedbd.com/  
Theme Version : 1  

This theme design based on S-Cart syetem. I will keep update this theme.  

Theme install : https://s-cart.org/docs/4.5/install-template.html  

# Install manual:  

Extracting the SCart template file has 2 folders:  
- public: Contains static files. For example images, javascript, css  
- src: Contains the main code of the interface  
The configuration file of the template is "src/config.json"  
The contents of the config file contain important configuration information:  
>"configKey": "ScartDefault", -> is the key of the template  

Copy the files in the directory "public" to "public/templates/ScartDefault"  
Copy the files in the directory "src" to "resources/views/templates/ScartDefault"  
With "ScartDefault" is the value defined in the file "config.json"  

 
# Note:   
Change made vendor s-cart folder match with theme design. This chage will show on Product detail page.
Location :  
>Core/src/library/helpers/price.php  
Old Code :  
>$html = $tmpAtt[0].'<span class="option_price">(+'.sc_currency_render($add_price,$currency, $rate).')</span>';  
Replace Code : >$html = $tmpAtt[0].'<sup>(+'.sc_currency_render($add_price,$currency, $rate).')</sup>';  
line No: 30  
**If you want don't wanat to chage, you can leave as it is. It will not effect the theme. But if you do, you have to change that code everytime update or install your comoper.**
