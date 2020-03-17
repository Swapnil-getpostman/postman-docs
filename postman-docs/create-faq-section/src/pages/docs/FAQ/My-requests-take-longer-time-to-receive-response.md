---
title: "My requests take longer time to receive response"
order: 2
page_id: "My requests take longer time to receive response"
warning: false
---

### My requests take longer time to receive response

After sending a request in Postman, application hangs / blank screen / black window / takes a lot of time to get a response? If you are receiving a blank screen / black window while opening the application or without sending any request, please try disabling the GPU as mentioned in this article [here.](https://support.getpostman.com/hc/en-us/articles/360026088854-Postman-window-is-blank)

If the issue is after sending a particular request, then please check on the size of the response you are receiving.

![ResponseSize.png](https://support.getpostman.com/hc/article_attachments/360043627853/ResponseSize.png)

In the latest version v7.3.5, the response time is longer and status code displays earlier than the response, as it relatively takes a longer time to load large responses on the application. We also have a limit of 50mb response that can be safely viewed. By default, we do not load response larger than 50mb. But if it extends, 100 MB is maximum buffer we currently have, so you can still change the response size up to 100 by navigating to **Settings > General Tab > Max response size in MB.**

![MaxResponseSize.png](https://support.getpostman.com/hc/article_attachments/360042787194/MaxResponseSize.png)

If your response exceeds 100+ MB, it is probably not going to succeed. But as a workaround, you can try the "Send and Download" option when running the request which should help you.  
  
We are currently working on handling large responses and the issue is being publicly tracked on our GitHub link [here](https://github.com/postmanlabs/postman-app-support/issues/4751).
