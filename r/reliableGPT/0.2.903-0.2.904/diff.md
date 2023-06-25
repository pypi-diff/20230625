# Comparing `tmp/reliableGPT-0.2.903.tar.gz` & `tmp/reliableGPT-0.2.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliableGPT-0.2.903.tar", last modified: Fri Jun 23 22:46:25 2023, max compression
+gzip compressed data, was "reliableGPT-0.2.904.tar", last modified: Sun Jun 25 00:50:46 2023, max compression
```

## Comparing `reliableGPT-0.2.903.tar` & `reliableGPT-0.2.904.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.539567 reliableGPT-0.2.903/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.903/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 22:46:25.539477 reliableGPT-0.2.903/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.903/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.538647 reliableGPT-0.2.903/reliableGPT.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      270 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-23 22:46:25.000000 reliableGPT-0.2.903/reliableGPT.egg-info/top_level.txt
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-23 22:46:25.539209 reliableGPT-0.2.903/reliablegpt/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.903/reliablegpt/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     9951 2023-06-23 22:32:41.000000 reliableGPT-0.2.903/reliablegpt/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7603 2023-06-23 22:41:56.000000 reliableGPT-0.2.903/reliablegpt/tests_main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-23 22:46:25.539598 reliableGPT-0.2.903/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-23 22:46:07.000000 reliableGPT-0.2.903/setup.py
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985941 reliableGPT-0.2.904/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-06-20 20:42:37.000000 reliableGPT-0.2.904/LICENSE
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-25 00:50:46.985836 reliableGPT-0.2.904/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     4077 2023-06-22 19:05:34.000000 reliableGPT-0.2.904/README.md
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985169 reliableGPT-0.2.904/reliableGPT.egg-info/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      220 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/PKG-INFO
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      270 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/requires.txt
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       12 2023-06-25 00:50:46.000000 reliableGPT-0.2.904/reliableGPT.egg-info/top_level.txt
+drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-06-25 00:50:46.985587 reliableGPT-0.2.904/reliablegpt/
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       87 2023-06-20 20:42:37.000000 reliableGPT-0.2.904/reliablegpt/__init__.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12007 2023-06-25 00:50:20.000000 reliableGPT-0.2.904/reliablegpt/main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)     7964 2023-06-24 23:16:21.000000 reliableGPT-0.2.904/reliablegpt/tests_main.py
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-06-25 00:50:46.985980 reliableGPT-0.2.904/setup.cfg
+-rw-r--r--   0 ishaanjaffer   (501) staff       (20)      331 2023-06-25 00:50:28.000000 reliableGPT-0.2.904/setup.py
```

### Comparing `reliableGPT-0.2.903/LICENSE` & `reliableGPT-0.2.904/LICENSE`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.903/README.md` & `reliableGPT-0.2.904/README.md`

 * *Files identical despite different names*

### Comparing `reliableGPT-0.2.903/reliablegpt/main.py` & `reliableGPT-0.2.904/reliablegpt/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -120,79 +120,144 @@
     result = fallback_request(args=args, kwargs=kwargs, fallback_strategy=fallback_strategy, self=self)
     if result == None:
         return graceful_string
     else:
         return result
     return graceful_string
 
-def capture_relevant_info(self, args, kwargs, result=None):
-    #print(f"In capture relevant info {kwargs['metadata']}")
-    return
-
+## Additional Features
+## Log OpenAI request, results and exceptions
+def capture_relevant_info(self, args, kwargs, result=None, error=None):
+    if 'reliableGPT_metadata' in kwargs:
+        print(f"In capture relevant info")
+
+        url = "http://0.0.0.0:5000/log_request"  # Replace with the actual URL of the endpoint
+
+        data = {
+            "metadata": kwargs['reliableGPT_metadata'],
+            "user_email": self.user_email,
+            "openai_create_function": str(self.openai_create_function),
+            "kwargs": kwargs,
+            "args": args,
+            "response": result,
+            "error": error
+        }
+        # print(f"In capture relevant info {data}")
+        response = requests.post(url, json=data)
+        # Check the response status
+        if response.status_code == 200:
+            print("POST request successful")
+        else:
+            print("POST request failed")
+        return
+
+# Parent Logging function
+def save_request(self, args, kwargs, posthog_event="", result="", posthog_metadata={}, errors=[]):
+    try:
+        #metadata  = kwargs['metadata']
+        capture_relevant_info(self, args, kwargs, result, errors) # log event before and after for reliableGPT users
+        if posthog_event != "":
+            posthog.capture(self.user_email, posthog_event, posthog_metadata) # save posthog event 
+
+        if result == self.graceful_string or len(errors) == 2: # returns a graceful string or got a 2nd exception
+            # send an email and alert
+            send_emails_task(self.user_email, posthog_metadata, self.send_notification)
+    except:
+        return # safe function, should not impact error handling if logging fails
 
 class reliableGPT:
     def __init__(
             self, 
             openai_create_function, 
             fallback_strategy = ['gpt-3.5-turbo', 'text-davinci-003', 'gpt-4', 'text-davinci-002'], 
             graceful_string="Sorry, the OpenAI API is currently down", 
             user_email="", 
             user_token="",
-            send_notification=False
+            send_notification=False,
+            open_ai_limits={}
             ):
         self.openai_create_function = openai_create_function
         self.graceful_string = graceful_string
         self.fallback_strategy = fallback_strategy
         self.user_email = user_email
         self.user_token = user_token
         self.send_notification = send_notification
+        self.open_ai_limits = open_ai_limits
 
         if self.user_email == "":
             raise ValueError("ReliableGPT Error: Please pass in a user email")
 
+
+    def handle_exception(self, args, kwargs, e):
+        result = self.graceful_string # default to graceful string
+        try:
+            # Attempt No. 1, exception is received from OpenAI 
+            print(colored(f"ReliableGPT: Error Response from {self.openai_create_function}", 'red'))
+            print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
+            result = handle_openAI_error(
+                args = args,
+                kwargs = kwargs,
+                openAI_error = e,
+                fallback_strategy = self.fallback_strategy,
+                graceful_string = self.graceful_string,
+                user_email = self.user_email,
+                user_token=self.user_token,
+                self=self
+            )
+            print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
+            if result == self.graceful_string:
+                # did a retry but still returned graceful string
+                save_request(
+                    self, 
+                    args, 
+                    kwargs,
+                    posthog_event = 'reliableGPT.recovered_request_exception', 
+                    result = result, 
+                    posthog_metadata = {'error':str(e), 'recovered_response': result}, 
+                    errors = [e]
+                )
+            else:
+                # No errors, successfull retry
+                save_request(
+                    self,
+                    args, 
+                    kwargs, 
+                    posthog_event = "reliableGPT.recovered_request", 
+                    result=result, 
+                    posthog_metadata={'error':str(e), 'recovered_response': result},
+                    errors = [e]
+                )
+        except Exception as e2:
+            # Exception 2, After trying to rescue
+            save_request(
+                self, 
+                args, 
+                kwargs, 
+                posthog_event = 'reliableGPT.recovered_request_exception',
+                result = "",
+                posthog_metadata = {'original_error':str(e), 'error2':str(e2), 'recovered_response': self.graceful_string},
+                errors = [e, e2]
+            )
+            return result
+        return result
+
+    ## Code that handles / wraps openai calls
     def __call__(self, *args, **kwargs):
-        start_time = time.time()
         try:
-            print("in call for normal case")
-            capture_relevant_info(self, args, kwargs)
-            posthog.capture(self.user_email, 'reliableGPT.request')
+            save_request(self, args, kwargs, "reliableGPT.request", result="")
             result = self.openai_create_function(*args, **kwargs)
-            capture_relevant_info(self, args, kwargs, result)
-
+            save_request(self, args, kwargs, "", result=result)
             return result
         except Exception as e:
-            result = self.graceful_string # default to graceful string
-            try:
-                print(colored(f"ReliableGPT: Error Response from {self.openai_create_function}", 'red'))
-                print(colored(f"ReliableGPT: Got Exception {e}", 'red'))
-                result = handle_openAI_error(
-                    args = args,
-                    kwargs = kwargs,
-                    openAI_error = e,
-                    fallback_strategy = self.fallback_strategy,
-                    graceful_string = self.graceful_string,
-                    user_email = self.user_email,
-                    user_token=self.user_token,
-                    self=self
-                )
-                print(colored(f"ReliableGPT: Recovered got a successful response {result}", "green"))
-                if result == self.graceful_string:
-                    send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Normal Retry"}, self.send_notification)
-                    posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'error':str(e), 'recovered_response': result})
-                    capture_relevant_info(self, args, kwargs, result)
-                else:
-                    posthog.capture(self.user_email, 'reliableGPT.recovered_request', {'error':str(e), 'recovered_response': result})
-                    capture_relevant_info(self, args, kwargs, result)
-            except Exception as e2:
-                posthog.capture(self.user_email, 'reliableGPT.recovered_request_exception', {'original_error':str(e), 'error2':str(e2), 'recovered_response': self.graceful_string})
-                send_emails_task(self.user_email, {"kwargs": kwargs, "OpenAI Error": e, "Type": "Got Exception on Retry", "error2": e2}, self.send_notification)
-                capture_relevant_info(self, args, kwargs, result)
-                return result
+            return self.handle_exception(args, kwargs, e)
+
+
 
 
+### OpenAI Key Management - Optional code if you want to use reliableGPT for Key Mgmt ###
 def add_keys(user_email="", keys=[]):
     url = f"https://reliable-gpt-backend-9gus.zeet-berri.zeet.app/add_keys"
     if user_email == "":
         return "reliableGPT: Please add an Email to add your keys"
     if len(keys) == 0:
         return "reliableGPT: Please add keys to add"
     payload = {"user_email": user_email}
```

### Comparing `reliableGPT-0.2.903/reliablegpt/tests_main.py` & `reliableGPT-0.2.904/reliablegpt/tests_main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,88 +1,96 @@
 import openai
-from reliablegpt import reliableGPT
-
+from main import reliableGPT
+import uuid
 
+openai.api_key = "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"
 from tenacity import retry, stop_after_attempt, wait_random_exponential
 
 # make openAI reliable and safe
 openai.ChatCompletion.create = reliableGPT(openai.ChatCompletion.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
 openai.Completion.create = reliableGPT(openai.Completion.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
 openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "ishaan@berri.ai", user_token = "AxQgeB3aEDK2B3x4fNG3ZYJRvFfOfQuCTOR83Y_9y5g", send_notification=True)
 
 def open_ai_completion_call():
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
-        {"role": "user", "content": "Who won the world series in 2020?"*400},
+        {"role": "user", "content": "Who won the world series in 2020?"},
         {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
         {"role": "user", "content": "Where was it played?"}
     ]
     temperature = 0.7
+    metadata = {
+        "request_uuid": str(uuid.uuid4()),  # Generate a new UUID for each request
+        "user": "ishaan@berri.ai"
+    }
     response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
     print(response)
 
 
 @retry(wait=wait_random_exponential(min=1, max=20), stop=stop_after_attempt(6))
 def get_embedding(text, model="text-embedding-ada-002", metadata={}):
   text = text.replace("\n", " ")
   return openai.Embedding.create(input=[text],
-                                 model=model)["data"][0]["embedding"]
+                                 model=model, metadata=metadata)["data"][0]["embedding"]
 
 def open_ai_embed_call():
     # openai.Embedding.create = reliableGPT(openai.Embedding.create, user_email= "ishaan@berri.ai", user_token = 'QA5T6lYfzB-8u3gFlC0hxtBZ-TbkJRF_FwrCB8GKTLM', send_notification=True)
     text = """
     Write in less than 25 words a hyper contextualized message about your company and how what your company does could help the visiting company's product offering. Start the message with a lowercase letter.
 Reference previous successful chat conversations for the tone and voice. Mix up the language. Try saying something new to each visitor. Make sure it makes sense. Be as specific as possible. If you don't know the person or the company then write a funny
 joke based on the person's location. If you don't have the person's location then write a message based on the information of the page the person is on. If you know the person's company mention the person's company in the message. If you don't know the company
 then don't mention it. Take into account previous chat history and context around the company and the visitor. Do not include any urls in the response.
 At the very end of the message say "(not a bot btw, real person)". Speak succinctly as you would to your best friend.
 Your response to the visitor on the site should be as helpful as possible. If you know the company the person works for or the person's name, include the first name or company name in the message.
 If the person's name or company is not known, then start the message with "hey!" Craft the style of your message as the best sales development representative in the world would write.
 Do not say the same message twice to the person. Start the response with a lowercase letter. Do not start a new conversation or message the person if you've already messaged them within 72 hours.
     """
     metadata = {
-        "instance": 123, 
-        "user": "ishaan@berri.ai"
+                "request_uuid": "40ae3a49-8a01-4c47-9985-6f22bca8c5b6", 
+                "user": "ishaan@berri.ai"
     }
-    embedding_result = get_embedding(text)
+    embedding_result = get_embedding(text, metadata=metadata)
     print(embedding_result)
     return embedding_result
 
 
 import concurrent.futures
 
 def test_multiple_calls():
     model = "gpt-4"
     messages = [
         {"role": "system", "content": "You are a helpful assistant."},
-        {"role": "user", "content": "Who won the world series in 2020?"*400},
+        {"role": "user", "content": "Who won the world series in 2020?" * 600},
         {"role": "assistant", "content": "The Los Angeles Dodgers won the World Series in 2020."},
         {"role": "user", "content": "Where was it played?"}
     ]
     temperature = 0.7
 
     error_count = 0
     failure_count = 0  # Track the number of failures
 
     def call_reliable_openai():
         nonlocal error_count, failure_count
         try:
             print("Making OpenAI Call")
+
             response = openai.ChatCompletion.create(model=model, messages=messages, temperature=temperature)
+            print(response)
             if response and "error" in response:
                 error_count += 1
             if response == "Sorry, the OpenAI (GPT) failed":
                 failure_count += 1
+
         except Exception as e:
             print("Exception occurred:", e)
             error_count += 1
 
     # Create a ThreadPoolExecutor with a maximum of 10 threads
-    with concurrent.futures.ThreadPoolExecutor(max_workers=10) as executor:
+    with concurrent.futures.ThreadPoolExecutor(max_workers=2) as executor:
         # Submit the callable to the executor for each call
         future_calls = [executor.submit(call_reliable_openai) for _ in range(20)]
 
         # Wait for all the futures to complete
         concurrent.futures.wait(future_calls)
 
     print(f"Error Count: {error_count}")
@@ -156,10 +164,11 @@
         text = text.replace("\n", " ")
         print("text")
         return openai.Embedding.create(input=[text],
                                         model=model)["data"][0]["embedding"]
     result = get_embedding("GM")
     #print(f"This is the embedding response {result}")
 
+#open_ai_completion_call()
 #test_embedding_bad_key()
 #open_ai_embed_call()
-#test_multiple_calls()
+test_multiple_calls()
```

