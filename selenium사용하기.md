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

자꾸 이런 오류가 나는데, 도대체 왜인지 모르겠다. 분명 경로는 확실한데, 권한이 없어서 그런 것 같지만 다른것들을 해도 잘 안된다 T^T
