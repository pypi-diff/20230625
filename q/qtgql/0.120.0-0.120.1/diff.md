# Comparing `tmp/qtgql-0.120.0.tar.gz` & `tmp/qtgql-0.120.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.120.0.tar", max compression
+gzip compressed data, was "qtgql-0.120.1.tar", max compression
```

## Comparing `qtgql-0.120.0.tar` & `qtgql-0.120.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1064 2023-06-21 14:34:56.020885 qtgql-0.120.0/LICENSE
--rw-r--r--   0        0        0     1805 2023-06-21 14:34:56.020885 qtgql-0.120.0/README.md
--rw-r--r--   0        0        0     4428 2023-06-21 14:35:17.905132 qtgql-0.120.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0     1919 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/config.py
--rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/__init__.py
--rw-r--r--   0        0        0     1548 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/cppref.py
--rw-r--r--   0        0        0       41 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/exceptions.py
--rw-r--r--   0        0        0     3105 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/graphql_ref.py
--rw-r--r--   0        0        0     1179 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/core/template.py
--rw-r--r--   0        0        0     3226 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/generator.py
--rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/__init__.py
--rw-r--r--   0        0        0     4207 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/definitions.py
--rw-r--r--   0        0        0    13536 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/evaluation.py
--rw-r--r--   0        0        0      749 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/operation/template.py
--rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/__init__.py
--rw-r--r--   0        0        0     4164 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/definitions.py
--rw-r--r--   0        0        0     8458 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/evaluation.py
--rw-r--r--   0        0        0     1625 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/schema/template.py
--rw-r--r--   0        0        0      445 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0     1524 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
--rw-r--r--   0        0        0     3059 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     1187 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
--rw-r--r--   0        0        0     2330 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
--rw-r--r--   0        0        0     2930 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.cpp
--rw-r--r--   0        0        0     4806 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     3250 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0    16334 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/types.py
--rw-r--r--   0        0        0     1151 2023-06-21 14:34:56.032885 qtgql-0.120.0/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-25 13:18:59.814578 qtgql-0.120.1/LICENSE
+-rw-r--r--   0        0        0     1805 2023-06-25 13:18:59.814578 qtgql-0.120.1/README.md
+-rw-r--r--   0        0        0     4428 2023-06-25 13:19:17.118449 qtgql-0.120.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0     1919 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/__init__.py
+-rw-r--r--   0        0        0     1548 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/cppref.py
+-rw-r--r--   0        0        0       41 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/exceptions.py
+-rw-r--r--   0        0        0     3105 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/graphql_ref.py
+-rw-r--r--   0        0        0     1179 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/core/template.py
+-rw-r--r--   0        0        0     3226 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/generator.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/__init__.py
+-rw-r--r--   0        0        0     4207 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/definitions.py
+-rw-r--r--   0        0        0    13536 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/evaluation.py
+-rw-r--r--   0        0        0      749 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/operation/template.py
+-rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/__init__.py
+-rw-r--r--   0        0        0     4164 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/definitions.py
+-rw-r--r--   0        0        0     8512 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/evaluation.py
+-rw-r--r--   0        0        0     1625 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/schema/template.py
+-rw-r--r--   0        0        0      445 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0     1527 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp
+-rw-r--r--   0        0        0     3059 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     1187 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp
+-rw-r--r--   0        0        0     2182 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp
+-rw-r--r--   0        0        0     3223 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.cpp
+-rw-r--r--   0        0        0     5130 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     3482 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0    16797 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/types.py
+-rw-r--r--   0        0        0     1151 2023-06-25 13:18:59.826578 qtgql-0.120.1/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2746 1970-01-01 00:00:00.000000 qtgql-0.120.1/PKG-INFO
```

### Comparing `qtgql-0.120.0/LICENSE` & `qtgql-0.120.1/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/README.md` & `qtgql-0.120.1/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/pyproject.toml` & `qtgql-0.120.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.120.0"
+version = "0.120.1"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/cli.py` & `qtgql-0.120.1/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/config.py` & `qtgql-0.120.1/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/core/cppref.py` & `qtgql-0.120.1/qtgqlcodegen/core/cppref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/core/graphql_ref.py` & `qtgql-0.120.1/qtgqlcodegen/core/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/core/template.py` & `qtgql-0.120.1/qtgqlcodegen/core/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/generator.py` & `qtgql-0.120.1/qtgqlcodegen/generator.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/operation/definitions.py` & `qtgql-0.120.1/qtgqlcodegen/operation/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/operation/evaluation.py` & `qtgql-0.120.1/qtgqlcodegen/operation/evaluation.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/operation/template.py` & `qtgql-0.120.1/qtgqlcodegen/operation/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/schema/definitions.py` & `qtgql-0.120.1/qtgqlcodegen/schema/definitions.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/schema/evaluation.py` & `qtgql-0.120.1/qtgqlcodegen/schema/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
 
     ret = QtGqlObjectType(
         name=t_name,
         interfaces_raw=options.implements,
         docstring=type_.description,
         fields_dict=options.all_fields,
         unique_fields=options.unique_fields,
+        is_root=t_name in type_info.root_types_names,
     )
     type_info.add_objecttype(ret)
     for interface in type_.interfaces:
         qtgql_interface = _evaluate_interface_type(type_info, interface)
         qtgql_interface.implementations[type_.name] = ret
     return ret
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/schema/template.py` & `qtgql-0.120.1/qtgqlcodegen/schema/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/macros/concrete_type_fields.jinja.hpp`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 {% endif -%}
 {% if f.is_custom_scalar -%}
 return 👉 f_private_name 👈.to_qt();
 {% else -%}
 return 👉 f_private_name 👈;
 {% endif -%}
 }
-void 👉 f.setter_name 👈(const 👉 f.type.member_type 👈 &v {% if f.arguments and type.implements_node %}, 👉 f.arguments_type 👈 args {% endif %})
+void 👉 f.setter_name 👈(const 👉 f.type.member_type_arg 👈 v {% if f.arguments and type.implements_node %}, 👉 f.arguments_type 👈 args {% endif %})
 {
 {%- if f.arguments and type.implements_node -%}
 {% set f_private_name %}👉 f.private_name 👈[args]{% endset %}
 {% else -%}
 {% set f_private_name %}👉 f.private_name 👈{% endset %}
 {% endif -%}
 👉 f_private_name 👈 = v;
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/macros/deserialize_concrete_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/macros/initialize_proxy_field.jinja.hpp`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/macros/update_concrete_field.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -20,29 +20,28 @@
 auto new_👉f_concrete.name👈 = data.value("👉f_concrete.name👈").👉 proxy_field.type.is_builtin_scalar.from_json_convertor 👈;
 if (👉current👈 != new_👉f_concrete.name👈){
 inst->👉fset_name👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
 {% endif %}
 {% elif proxy_field.type.is_custom_scalar %}
 auto new_👉proxy_field.name👈 = 👉 proxy_field.type.is_custom_scalar.type_name() 👈();
-new_👉proxy_field.name👈.deserialize(data.value("👉proxy_field.name👈"));
+new_👉proxy_field.name👈.deserialize(data.value("👉f_concrete.name👈"));
 if (👉current👈 != new_👉proxy_field.name👈){
 inst->👉fset_name👈(new_👉f_concrete.name👈 👉 setter_end 👈);
 }
 {% elif proxy_field.type.is_queried_object_type %}
 {% if f_concrete.implements_node %}
 auto 👉f_concrete.name👈_data = data.value("person").toObject();
 if (👉current👈 && 👉current👈->get_id() == 👉f_concrete.name👈_data.value("id").toString()){
 👉proxy_field.type.updater_name👈(👉current👈, 👉f_concrete.name👈_data,  👉operation_pointer👈);
 }
 else{
-inst->👉fset_name👈(👉proxy_field.type.deserializer_name👈(👉f_concrete.name👈_data, 👉operation_pointer👈) 👉 setter_end 👈);
+inst->👉fset_name👈(👉proxy_field.type.deserializer_name👈(data.value("👉f_concrete.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
 }
 {% endif %}
-inst->👉fset_name👈(👉proxy_field.type.deserializer_name👈(data.value("👉f_concrete.name👈").toObject(), 👉operation_pointer👈) 👉 setter_end 👈);
 {% else %}
 throw qtgql::exceptions::NotImplementedError({"👉proxy_field.type.__class__.__name__👈 is not supporting updates ATM"});
 {% endif %}
 }
 {% if proxy_field.type.is_optional %}
 else {
 inst->👉fset_name👈({} 👉 setter_end 👈);
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.cpp` & `qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -16,54 +16,63 @@
 throw qtgql::exceptions::InterfaceDeserializationError(tp_name.toStdString());
 }
 {% endfor %}
 
 
 {% for t in context.operation.narrowed_types %}
 // Constructor
+{% if t.concrete.is_root -%}
+👉 t.name 👈::👉 t.name 👈(👉 context.operation.name 👈 * operation): QObject::QObject(operation){
+    m_inst = 👉 t.concrete.name 👈::instance();
+    auto m_inst_ptr = m_inst;
+{% else -%}
 👉 t.name 👈::👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst)
 : m_inst{inst}, QObject::QObject(operation)
 {
-    Q_ASSERT_X(m_inst, __FILE__, "Tried to instantiate a proxy object with an empty pointer!");
-    auto inst_ptr = m_inst.get();
+    auto m_inst_ptr = m_inst.get();
+    Q_ASSERT_X(m_inst_ptr, __FILE__, "Tried to instantiate a proxy object with an empty pointer!");
+    {% endif -%}
     {%- for field in t.fields -%}
     👉 initialize_proxy_field(field) 👈
     {% endfor -%}
     {#- connecting signals here, when the concrete changed it will be mirrored here. -#}
     {%- for field in t.fields -%}
-    connect(m_inst.get(), &👉context.schema_ns👈::👉t.concrete.name👈::👉 field.concrete.signal_name 👈, this,
+    connect(m_inst_ptr, &👉context.schema_ns👈::👉t.concrete.name👈::👉 field.concrete.signal_name 👈, this,
             [&](){emit 👉 field.concrete.signal_name 👈();});
     {% endfor -%}
 
 }
 // Deserialzier
+{% if not t.concrete.is_root %}
 std::shared_ptr<👉 t.concrete.name 👈> 👉 t.deserializer_name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation){
 if (data.isEmpty()){
     return {};
 }
 {% if t.concrete.implements_node %}
 auto cached_maybe = 👉 t.concrete.name 👈::get_node(data.value("id").toString());
 if(cached_maybe.has_value()){
     auto node = cached_maybe.value();
     👉 t.updater_name 👈(node, data, operation);
     return node;
 }
 {% endif -%}
-auto inst = std::make_shared<👉 t.concrete.name 👈>();
+auto inst = 👉 t.concrete.name 👈::shared();
 {% for f in t.fields -%}
 {% set setter %}inst->👉 f.concrete.setter_name 👈{% endset %}
 👉deserialize_concrete_field(f, setter)👈
 {% endfor %}
 {% if t.concrete. implements_node %}
 👉 t.concrete.name 👈::ENV_CACHE()->add_node(inst);
 {% endif %}
 return inst;
 };
+{% endif %}
+
 // Updater
-void 👉 t.updater_name 👈(👉 t.concrete.member_type 👈 &inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation)
+void 👉 t.updater_name 👈(👉 t.concrete.member_type_arg 👈 inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation)
 {
 {%for f in t.fields -%}
 👉update_concrete_field(f,f.concrete, fset_name=f.concrete.setter_name, private_name=f.private_name, operation_pointer="operation")👈
 {% endfor %}
 };
 {% endfor %}
 }
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
 #include <QObject>
 
 namespace 👉 context.config.env_name 👈::👉context.ns👈{
 class 👉 context.operation.name 👈;
 
 namespace deserializers{
-{% for t in context.operation.narrowed_types -%}
+{% for t in context.operation.narrowed_types if not t.concrete.is_root -%}
 std::shared_ptr<👉 t.concrete.name 👈> des_👉 t.name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation);
 {% endfor -%}
 {% for t in context.operation.interfaces -%}
 std::shared_ptr<👉 t.concrete.name 👈> des_👉 t.name 👈(const QJsonObject& data, const 👉 context.operation.name 👈 * operation);
 {% endfor -%}
 };
 
 namespace updaters{
 {% for t in context.operation.narrowed_types -%}
-void update_👉 t.name 👈(👉 t.concrete.member_type 👈 &inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation);
+void update_👉 t.name 👈(👉 t.concrete.member_type_arg 👈 inst, const QJsonObject &data, const 👉 context.operation.name 👈 * operation);
 {% endfor -%}
 
 };
 
 // ------------ Narrowed Object types ------------
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈: public QObject{
@@ -38,24 +38,32 @@
 
 {# members #}
 {% if context.debug -%}
 public: // WARNING: members are public because you have debug=True in your config file.
 {% else %}
 protected:
 {% endif %}
+{% if t.concrete.is_root %}
+👉context.schema_ns👈::👉 t.concrete.name 👈 * m_inst;
+{% else %}
 const std::shared_ptr<👉context.schema_ns👈::👉 t.concrete.name 👈> m_inst;
+{% endif %}
 {% for ref_field in t.references -%}
 const 👉ref_field.property_type👈 m_👉ref_field.name👈 = {};
 {% endfor %}
 {%- for model_field in t.models -%}
 👉 model_field.property_type 👈 m_👉model_field.name👈;
 {% endfor %}
 
 public:
+{% if t.concrete.is_root %}
+👉 t.name 👈(👉 context.operation.name 👈 * operation);
+{% else %}
 👉 t.name 👈(👉 context.operation.name 👈 * operation, const std::shared_ptr<👉 t.concrete.name 👈> &inst);
+{% endif %}
 
 {% for f in t.fields -%}
 {%- if f.type.is_queried_object_type or f.type.is_model %}
 [[nodiscard]] inline const 👉 f.property_type 👈  👉 f.concrete.getter_name 👈() const {
     return m_👉f.name👈;
 {%- else -%}
 [[nodiscard]] inline const 👉 f.property_type 👈 👉 f.concrete.getter_name 👈() const {
@@ -117,15 +125,16 @@
 return m_operation_id;
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data){
         auto data = message.value("data").toObject();
-        m_data = new 👉 context.operation.root_type.name👈(this, 👉 context.operation.root_type.deserializer_name 👈(data, this));
+        👉 context.operation.root_type.updater_name👈(👉 context.operation.root_type.concrete.name👈::instance(), data, this);
+        m_data = new 👉 context.operation.root_type.name👈(this);
         emit dataChanged();
     }
     else{
     throw qtgql::exceptions::NotImplementedError({"Updates on root types is not implemented yet."});
     }
 }
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.120.1/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,25 @@
 class 👉 type.name 👈;
 {% endfor %}
 
 {% for type in context.types %}
 {%- set base_class -%}{% if type. implements_node %}NodeInterfaceABC{% else %}ObjectTypeABC{% endif %}{%- endset -%}
 class 👉 type.name 👈 {% for base in type.bases %}{%if loop.first%}: {% endif %} public 👉 base.name 👈 {% if not loop.last %}, {% endif %}{% endfor %}{
 Q_OBJECT
-
 👉 concrete_type_fields(type) 👈
 public:
+{% if type.is_root %} {# root types should be singletons #}
+[[nodiscard]] static 👉 type.name 👈* instance(){
+static 👉 type.name 👈 inst;
+return &inst;
+}
+{% else %}
+QTGQL_STATIC_MAKE_SHARED(👉 type.name 👈)
+{% endif %}
+
 👉 type.name 👈()= default;
 
 inline static const QString TYPE_NAME = "👉 type.name 👈";
 
 {% if type.implements_node -%}
 static std::optional<std::shared_ptr<👉 type.name 👈>> get_node(const QString & id){
     auto node = ENV_CACHE()->get_node(id);
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/types.py` & `qtgql-0.120.1/qtgqlcodegen/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,22 @@
         """
         :returns: The C++ type of the concrete instance member.
         """
         # Usually `type_name` should suffice, if the type needs to return something else this is overridden.
         return self.type_name()
 
     @property
+    def member_type_arg(self) -> str:
+        """
+
+        :return: The C++ member_type if it was passed in argument to somewhere.
+        """
+        return self.member_type
+
+    @property
     def fget_type(self) -> str:
         """
 
         :return: type for the proxy object, usually this would be the member type though for custom scalars
         there is `to_qt` that has different type.
         """
         return self.member_type
@@ -236,14 +244,15 @@
         return tuple(self.fields_dict.values())
 
 
 @define(slots=False)
 class QtGqlObjectType(BaseQtGqlObjectType):
     interfaces_raw: tuple[QtGqlInterface, ...] = attrs.Factory(tuple)
     unique_fields: tuple[QtGqlFieldDefinition, ...] = attrs.Factory(tuple)
+    is_root: bool = False
 
     def implements(self, interface: QtGqlInterface) -> bool:
         for m_interface in self.interfaces_raw:
             if interface is m_interface or m_interface.implements(interface):
                 return True
         return False
 
@@ -297,16 +306,23 @@
         return self
 
     def type_name(self) -> str:
         return self.name
 
     @property
     def member_type(self) -> str:
+        if self.is_root:
+            return self.type_name()  # root types are singletons
         return f"std::shared_ptr<{self.type_name()}>"
 
+    @property
+    def member_type_arg(self) -> str:
+        pointer_type = "*" if self.is_root else "&"
+        return f"{self.member_type} {pointer_type}"
+
     def __attrs_post_init__(self):
         # inject this object type to the interface.
         # later the interface would use this list to know who he might resolve to.
         for base in self.interfaces_raw:
             if not base.implementations.get(self.name):
                 base.implementations[self.name] = self
```

### Comparing `qtgql-0.120.0/qtgqlcodegen/utils.py` & `qtgql-0.120.1/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.120.0/PKG-INFO` & `qtgql-0.120.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.120.0
+Version: 0.120.1
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

