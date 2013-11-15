flask-postmark
==============

flask配置文件中设置：

   POSTMARK_API_KEY    = 'your-key'
   
   POSTMARK_SENDER     = 'sender@signature.com'
   
   POSTMARK_TEST_MODE  = [True/False]
    

初始化：

   mail = Postmark()
   
   mail.init_app(current_app)

发送：

   pm = mail.create_mail(to="to@mail.com", subject="subject", tag="tag", html_body="hello postmark")
   
   pm.send()
  
  
