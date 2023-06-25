# Comparing `tmp/llm_few_shot_gen-0.0.2.tar.gz` & `tmp/llm_few_shot_gen-0.0.3.tar.gz`

## Comparing `llm_few_shot_gen-0.0.2.tar` & `llm_few_shot_gen-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/.idea/llm-few-shot-gen.iml
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/.idea/modules.xml
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/notebooks/few_shot_shirt_designs.ipynb
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/notebooks/.ipynb_checkpoints/few_shot_shirt_designs-checkpoint.ipynb
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/context/__init__.py
--rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/context/midjourney.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/few_shot_examples/__init__.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/few_shot_examples/midjourney.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/few_shot_examples/utils.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/__init__.py
--rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/base.py
--rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/midjourney.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/prompt.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/models/__init__.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/models/generator.py
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/models/output.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/README.md
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/run_build_and_publish.sh
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/.idea/llm-few-shot-gen.iml
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/notebooks/few_shot_shirt_designs.ipynb
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/notebooks/.ipynb_checkpoints/few_shot_shirt_designs-checkpoint.ipynb
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/context/__init__.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/context/midjourney.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/few_shot_examples/__init__.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/few_shot_examples/midjourney.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/few_shot_examples/utils.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/__init__.py
+-rw-r--r--   0        0        0     5025 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/base.py
+-rw-r--r--   0        0        0     3227 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/midjourney.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/prompt.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/models/__init__.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/models/generator.py
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/models/output.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/LICENSE.txt
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/README.md
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 llm_few_shot_gen-0.0.3/PKG-INFO
```

### Comparing `llm_few_shot_gen-0.0.2/.idea/llm-few-shot-gen.iml` & `llm_few_shot_gen-0.0.3/.idea/llm-few-shot-gen.iml`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/.idea/inspectionProfiles/Project_Default.xml` & `llm_few_shot_gen-0.0.3/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/notebooks/few_shot_shirt_designs.ipynb` & `llm_few_shot_gen-0.0.3/notebooks/few_shot_shirt_designs.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9883928571428572%*

 * *Differences: {"'cells'": "{6: {'source': ['## Add Few Shot examples']}, delete: [7]}",*

 * * "'metadata'": "{'language_info': {'version': '3.9.13'}}"}*

```diff
@@ -63,23 +63,15 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f045ca3f-4ee2-48e9-9afe-b56217e87eb2",
             "metadata": {},
             "source": [
-                "## Add context and few shot examples"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f7c3993b-3cdb-4eec-b9e4-7349de33e6e6",
-            "metadata": {},
-            "source": [
-                "### Context of Midjourney"
+                "## Add Few Shot examples"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ae75a067-2098-4844-8ac9-2a218df43e8d",
             "metadata": {},
             "source": [
@@ -211,13 +203,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `llm_few_shot_gen-0.0.2/notebooks/.ipynb_checkpoints/few_shot_shirt_designs-checkpoint.ipynb` & `llm_few_shot_gen-0.0.3/notebooks/.ipynb_checkpoints/few_shot_shirt_designs-checkpoint.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9740703925884591%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'source': {insert: [(1, 'from IPython.display import "*

 * *            "JSON\\n'), (2, 'from langchain.chat_models import ChatOpenAI\\n'), (3, 'from "*

 * *            'llm_few_shot_gen.few_shot_examples.utils import '*

 * *            "get_shirt_design_prompt_examples\\n'), (4, 'from llm_few_shot_gen.generators import "*

 * *            "MidjourneyPromptGenerator\\n'), (5, 'from llm_few_shot_gen.models.output import "*

 * *            "ImagePromptOutputModel')], delete: [3, 2, 1]}}, 4: {'ex […]*

```diff
@@ -16,91 +16,75 @@
             "source": [
                 "## Setup\n",
                 "import required modules and create MidjourneyPromptGenerator instance"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 1,
             "id": "1dea6131-02aa-43f0-bd10-dde7bf849715",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
-                "from llm_few_shot_gen.prompt.midjourney.utils import get_shirt_design_prompt_examples\n",
-                "from llm_few_shot_gen.langchain_fns import get_chat_gpt_model\n",
-                "from llm_few_shot_gen.prompt.midjourney import MidjourneyPromptGenerator"
+                "from IPython.display import JSON\n",
+                "from langchain.chat_models import ChatOpenAI\n",
+                "from llm_few_shot_gen.few_shot_examples.utils import get_shirt_design_prompt_examples\n",
+                "from llm_few_shot_gen.generators import MidjourneyPromptGenerator\n",
+                "from llm_few_shot_gen.models.output import ImagePromptOutputModel"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "35cd77ee-bc80-4964-b7fd-52b19ae4f5ea",
             "metadata": {},
             "source": [
                 "Add your open ai key from https://platform.openai.com/account/api-keys"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 14,
             "id": "ccea7c22-60aa-4917-ba77-8bc691fcab64",
             "metadata": {},
             "outputs": [],
             "source": [
                 "os.environ[\"OPENAI_API_KEY\"] = \"\""
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 15,
             "id": "8b4bb45a-769a-4944-b80f-2e9ab05bed35",
             "metadata": {},
             "outputs": [],
             "source": [
-                "llm = get_chat_gpt_model(temperature=0.7)\n",
+                "llm = ChatOpenAI(temperature=0.7)\n",
                 "prompt_generator = MidjourneyPromptGenerator(llm)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "f045ca3f-4ee2-48e9-9afe-b56217e87eb2",
             "metadata": {},
             "source": [
-                "## Add context and few shot examples"
-            ]
-        },
-        {
-            "cell_type": "markdown",
-            "id": "f7c3993b-3cdb-4eec-b9e4-7349de33e6e6",
-            "metadata": {},
-            "source": [
-                "### Context of Midjourney"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 4,
-            "id": "dd97bcdd-7a15-4e4b-95d8-fe94de24ef76",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "prompt_generator.set_context()"
+                "## Add Few Shot examples"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "ae75a067-2098-4844-8ac9-2a218df43e8d",
             "metadata": {},
             "source": [
                 "### Few shot prompt examples"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 16,
             "id": "97aad3cf-a3e6-43e4-91df-2284e4440049",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
@@ -118,15 +102,15 @@
                 "for i, example in enumerate(prompt_examples[0:3]):\n",
                 "    print(f\"Example {i}\")\n",
                 "    print(example)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 10,
+            "execution_count": 17,
             "id": "51e9c14b-a81d-475d-b765-308c0b62411f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "prompt_generator.set_few_shot_examples(prompt_examples)"
             ]
         },
@@ -137,43 +121,69 @@
             "source": [
                 "## Prompt generation playground\n",
                 "Choose a simple text which gets transformed into high quality midjournes prompt."
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 18,
             "id": "75e9c0dd-882a-476d-92d8-7f7b61b6053e",
             "metadata": {},
             "outputs": [],
             "source": [
-                "text = \"\"\"Sloth on tree cartoon\"\"\""
+                "text = \"\"\"Sloth on tree cartoon\"\"\"\n",
+                "parsed_output: ImagePromptOutputModel = prompt_generator.generate(text)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 13,
+            "execution_count": 19,
             "id": "9ff973a4-3358-49db-af29-dcf68baf0476",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [
                 {
                     "data": {
+                        "application/json": {
+                            "few_shot_artists": [
+                                "Studio Ghibli",
+                                "Gediminas Pranckevicius",
+                                "Moebius"
+                            ],
+                            "few_shot_styles": [
+                                "cartoonish",
+                                "minimalistic",
+                                "cyberpunk",
+                                "realistic"
+                            ],
+                            "image_prompts": [
+                                "A cartoonish sloth sitting on a tree branch, bright colors. T-shirt design graphic, vector, contour, white background, in the style of Studio Ghibli's enchanting artwork.",
+                                "A realistic sloth hanging upside down from a tree branch, t-shirt design graphic, vector, contour, white background, in the style of wildlife illustrations.",
+                                "A sloth sleeping on a tree branch, vector illustration, flat design, digital drawing, t-shirt design. Use a minimalistic style with soft, soothing colors.",
+                                "A cyberpunk sloth perched on a neon-lit tree, digital drawing, t-shirt design. Use a futuristic color palette and add some cyberpunk elements to the tree.",
+                                "A sloth with a kind facial expression hanging from a tree, airbrush art, fantasy art, t-shirt design. Use pastel hues and add some fantasy elements to the tree."
+                            ]
+                        },
                         "text/plain": [
-                            "'A sloth hanging upside down on a tree branch, surrounded by tropical foliage. The sloth is looking directly at the viewer, its eyes wide open, and its fur is soft and fluffy. The background is blurry, with a focus on the sloth, and there are dappled rays of sunlight filtering through the leaves. The image should be highly detailed and realistic.'"
+                            "<IPython.core.display.JSON object>"
                         ]
                     },
-                    "execution_count": 13,
-                    "metadata": {},
+                    "execution_count": 19,
+                    "metadata": {
+                        "application/json": {
+                            "expanded": false,
+                            "root": "root"
+                        }
+                    },
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "prompt_generator.generate(text)"
+                "JSON(parsed_output.dict())"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a16ac046-2e8c-46e5-8cc0-cd4bf463a921",
             "metadata": {},
@@ -193,13 +203,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.10"
+            "version": "3.9.13"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/context/midjourney.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/context/midjourney.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/few_shot_examples/midjourney.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/few_shot_examples/midjourney.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/base.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/base.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/midjourney.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/midjourney.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/generators/prompt.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/generators/prompt.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/src/llm_few_shot_gen/models/generator.py` & `llm_few_shot_gen-0.0.3/src/llm_few_shot_gen/models/generator.py`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/LICENSE.txt` & `llm_few_shot_gen-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `llm_few_shot_gen-0.0.2/pyproject.toml` & `llm_few_shot_gen-0.0.3/pyproject.toml`

 * *Files identical despite different names*

