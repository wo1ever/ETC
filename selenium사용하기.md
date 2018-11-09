₩₩₩
---------------------------------------------------------------------------
WebDriverException                        Traceback (most recent call last)
<ipython-input-48-d0e1bd25939b> in <module>()
----> 1 driver = webdriver.Chrome(executable_path='/Users/seyoung/Downloads/chromedriver')

/anaconda3/lib/python3.6/site-packages/selenium/webdriver/chrome/webdriver.py in __init__(self, executable_path, port, options, service_args, desired_capabilities, service_log_path, chrome_options, keep_alive)
     71             service_args=service_args,
     72             log_path=service_log_path)
---> 73         self.service.start()
     74 
     75         try:

/anaconda3/lib/python3.6/site-packages/selenium/webdriver/common/service.py in start(self)
    102             time.sleep(1)
    103             if count == 30:
--> 104                 raise WebDriverException("Can not connect to the Service %s" % self.path)
    105 
    106     def assert_process_still_running(self):

WebDriverException: Message: Can not connect to the Service /Users/seyoung/Downloads/chromedriver

₩₩₩

자꾸 이런 오류가 나는데, 도대체 왜인지 모르겠다. 분명 경로는 확실한데, 권한이 없어서 그런 것 같지만 다른것들을 해도 잘 안된다 T^T

1. 몇 시간동안 거의 모든 google관련 문서를 보았다. 그 결과 내가 할 수 있는 모든 일을 했다는 느낌이 들었다.
2. 결국 은정님과 데잇걸즈 분들께 질문을 남겼다.
3. 은정님께서 해보고 결과를 알려달라고 보내주셨던 것 중에, ₩vi etc/hosts₩를 실행했을 때 아무것도 안나온다는 문제점 발견
4. hosts파일 덮어씌우니 해결되었다!

이렇게 간단한것을.. 몇 시간동안 엄청나게 많은 것을 해보았다고 한다...!  
이제 본격 크롤링을 할 수 있게 되었다. 😭기뻐....
