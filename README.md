# DaumNews_crawl
다음뉴스를 크롤링하는 파이썬 코드입니다. / This is the python code that crawls the following news.

<h1>다음뉴스 크롤링</h1>
다음뉴스의 하이퍼 링크를 모두 출력해오는 코드입니다. 다른 크롤링과 다소 적어서 다르다고 느끼시겟지만, 
기본적인 원리만 담은 하이퍼링크를 출력해오는 코드입니다. 
우선 필요한 모듈은 'urllib' 과 'BeautifulSoup' 모듈을 불러옵니다.

그후 urllib 모듈의 기능인 urlopen기능을 사용하여 , 모든 하이퍼 링크를 불러옵니다.

<pre>
<code>
for link in bsObject.find_all('a'):
    print(link.text.strip(), link.get('href'))
    
</code>
</pre>

위에 코드를 해석해보자면 html에서 모든 a 로된 href 즉 하이퍼링크를 불러오라는겁니다.
이러한 원리로 출력을 해보면 <br> 모든 하이퍼링크가 출력이 됩니다.

모듈은 밑에 모듈을 다운받았습니다.
<pre>
<code>
pip install urllib.request
pip install BeautifulSoup
</code>
</pre>
제가 다음뉴스를 선택한이유는 처음에는 네이버뉴스(https://news.naver.com/)를 썻는데 출력이 안되는걸보니
네이버측에서 막은거 같습니다.

# DaumNews_crawl
<h4>All translations are written through Google Translator</h4>

This is the python code that crawls the following news. / This is the python code that crawls the following news.

<h1>Daum news crawl</h1>
This is the code that prints out all hyperlinks of Daum News. It's a little bit different from other crawls, so you might feel different,
This is a code that prints out a hyperlink that contains only basic principles.
First of all, the necessary modules are called'urllib' and'BeautifulSoup' modules.

After that, all hyperlinks are loaded using the urlopen function, a function of the urllib module.

<pre>
<code>
for link in bsObject.find_all('a'):
    print(link.text.strip(), link.get('href'))
    
</code>
</pre>

Interpreting the code above is to load all a hrefs or hyperlinks from html.
If you print with this principle, all hyperlinks will be printed.

I downloaded the module below.
<pre>
<code>
pip install urllib.request
pip install BeautifulSoup
</code>
</pre>
The reason I chose Daum News was that I initially used Naver News (https://news.naver.com/), but it was not possible to print it.
Naver seems to have blocked it.
