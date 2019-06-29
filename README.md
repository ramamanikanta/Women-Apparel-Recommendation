# Women-Apparel-Recommendation
Women Apparel Recommendations for data collected through Amazon Product API<br>
Data Source:Data  was retrieved from Amazon Product API with Womens tops filter<br>

<h2>Features</h1><br>
1. asin  ( Amazon standard identification number)<br>
2. brand ( brand to which the product belongs to )<br>
3. color ( Color information of apparel, it can contain many colors as   a value ex: red and black stripes )<br> 
4. product_type_name (type of the apperal, ex: SHIRT/TSHIRT )<br>
5. medium_image_url  ( url of the image )<br>
6. title (title of the product)<br>
7. formatted_price (price of the product)<br>

Applied Text processing techniques using NLTK like stopword removal,stemming.<br>

Applied Text based Product similarity techniques like on <Strong><i>"title"</i></Strong> feature<br>
<ul>
  <li>BagofWords</li>
<li>TF-IDF</li>
<li>IDF</li>
<li>Average-Word2Vec</li>
<li>TF-IDF weighted Word2Vec</li>
<li>IDF weighted Word2Vec</li>
  </ul>

Combined the above techniques with <Strong><i>"brand"</i></Strong> and <Strong><i>"color"</i></Strong> features to achieve product similarity based on "Brand" and "Color" by tweaking the weights for every feature.<br>

Applied CNN for finding Image-based product similarities<br>
Converted the product images using <strong>VGG-16</strong> CNN for image feature extraction.<br>
Used Keras "ImageDataGenerator" with Tensorflow backend for image processing and finding similarities.<br>

For all the above techniques used <Strong>Eucledian</Strong> distance as a measure for finding similarities


