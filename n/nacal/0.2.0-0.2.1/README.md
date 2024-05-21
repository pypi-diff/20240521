# Comparing `tmp/nacal-0.2.0.tar.gz` & `tmp/nacal-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nacal-0.2.0.tar", last modified: Fri May 17 14:06:23 2024, max compression
+gzip compressed data, was "nacal-0.2.1.tar", last modified: Tue May 21 19:01:23 2024, max compression
```

## Comparing `nacal-0.2.0.tar` & `nacal-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-17 14:06:23.023909 nacal-0.2.0/
--rw-r--r--   0 marcos    (1000) marcos    (1000)     4371 2024-05-17 14:06:23.023909 nacal-0.2.0/PKG-INFO
--rw-r--r--   0 marcos    (1000) marcos    (1000)     2969 2024-05-17 14:06:22.000000 nacal-0.2.0/README.md
-drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-17 14:06:23.019909 nacal-0.2.0/nacal/
--rw-r--r--   0 marcos    (1000) marcos    (1000)      184 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal/__init__.py
--rw-r--r--   0 marcos    (1000) marcos    (1000)   122922 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal/nacal.py
-drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-17 14:06:23.023909 nacal-0.2.0/nacal.egg-info/
--rw-r--r--   0 marcos    (1000) marcos    (1000)     4371 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal.egg-info/PKG-INFO
--rw-r--r--   0 marcos    (1000) marcos    (1000)      195 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal.egg-info/SOURCES.txt
--rw-r--r--   0 marcos    (1000) marcos    (1000)        1 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal.egg-info/dependency_links.txt
--rw-r--r--   0 marcos    (1000) marcos    (1000)       13 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal.egg-info/requires.txt
--rw-r--r--   0 marcos    (1000) marcos    (1000)        6 2024-05-17 14:06:22.000000 nacal-0.2.0/nacal.egg-info/top_level.txt
--rw-r--r--   0 marcos    (1000) marcos    (1000)       38 2024-05-17 14:06:23.023909 nacal-0.2.0/setup.cfg
--rw-r--r--   0 marcos    (1000) marcos    (1000)     1561 2024-05-17 14:06:22.000000 nacal-0.2.0/setup.py
+drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-21 19:01:23.657993 nacal-0.2.1/
+-rw-r--r--   0 marcos    (1000) marcos    (1000)     4322 2024-05-21 19:01:23.653993 nacal-0.2.1/PKG-INFO
+-rw-r--r--   0 marcos    (1000) marcos    (1000)     2920 2024-05-21 19:01:23.000000 nacal-0.2.1/README.md
+drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-21 19:01:23.653993 nacal-0.2.1/nacal/
+-rw-r--r--   0 marcos    (1000) marcos    (1000)      184 2024-05-21 19:01:22.000000 nacal-0.2.1/nacal/__init__.py
+-rw-r--r--   0 marcos    (1000) marcos    (1000)   127138 2024-05-21 19:01:22.000000 nacal-0.2.1/nacal/nacal.py
+drwxr-xr-x   0 marcos    (1000) marcos    (1000)        0 2024-05-21 19:01:23.653993 nacal-0.2.1/nacal.egg-info/
+-rw-r--r--   0 marcos    (1000) marcos    (1000)     4322 2024-05-21 19:01:23.000000 nacal-0.2.1/nacal.egg-info/PKG-INFO
+-rw-r--r--   0 marcos    (1000) marcos    (1000)      195 2024-05-21 19:01:23.000000 nacal-0.2.1/nacal.egg-info/SOURCES.txt
+-rw-r--r--   0 marcos    (1000) marcos    (1000)        1 2024-05-21 19:01:23.000000 nacal-0.2.1/nacal.egg-info/dependency_links.txt
+-rw-r--r--   0 marcos    (1000) marcos    (1000)       13 2024-05-21 19:01:23.000000 nacal-0.2.1/nacal.egg-info/requires.txt
+-rw-r--r--   0 marcos    (1000) marcos    (1000)        6 2024-05-21 19:01:23.000000 nacal-0.2.1/nacal.egg-info/top_level.txt
+-rw-r--r--   0 marcos    (1000) marcos    (1000)       38 2024-05-21 19:01:23.657993 nacal-0.2.1/setup.cfg
+-rw-r--r--   0 marcos    (1000) marcos    (1000)     1561 2024-05-21 19:01:23.000000 nacal-0.2.1/setup.py
```

### Comparing `nacal-0.2.0/PKG-INFO` & `nacal-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: nacal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Notacion Asociativa para un curso de Algebra Lineal (NAcAL)
 Home-page: https://github.com/mbujosab/nacallib
 Author: Marcos Bujosa
 Author-email: mbujosab@ucm.es
 License: GPLv3
-Description: [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
-        [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)\]\]
+Description: [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)
+        [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
         
         # Módulo "NAcAL" (Notación Asociativa para un Curso de Álgebra Lineal)
         
         Este módulo implementa la notación, los objetos y los procedimientos
         descritos en el
         [libro](https://mbujosab.github.io/CursoDeAlgebraLineal/libro.pdf) del
         [Curso de ÁLgebra
         Lineal](https://github.com/mbujosab/CursoDeAlgebraLineal)
         correspondiente a la asignatura [Matemáticas
         II.](https://www.ucm.es/fundamentos-analisis-economico2/algebra-2)
         
         Aunque es posible su uso desde un terminal, este módulo está pensado
         para ser empleado en [Notebooks de Jupyter](https://jupyter.org/) (y
-        también desde documentos de \(\LaTeX{}\)).
+        también desde documentos de LaTeX).
         
         Este módulo muestra cómo llegar a la mayoría de los resultados del curso
         de Álgebra Lineal empleando el método de eliminación. NAcAL no solo
         resuelve sistemas de ecuaciones, invierte matrices, calcula
         determinantes, diagonaliza matrices tanto por semejanza como por
         congruencia, etc. sino que muestra los pasos empleados para llegar al
         resultado como si se hiciera con lápiz y papel (ofreciendo el código
@@ -39,15 +39,15 @@
         La documentación explica la programación del código y sirve como
         material adicional al [libro del
         curso](https://github.com/mbujosab/CursoDeAlgebraLineal) (este módulo es
         una implementación literal de lo mostrado en dicho libro).
         
         Puede ver el uso del módulo sin necesidad de instalar nada, tan solo
         accediendo a los Notebooks de Jupyter alojados en
-        [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
+        [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
         con su navegador de páginas web (tenga en cuenta que MyBinder puede
         tardar unos minutos en cargar el módulo y el Notebook de demostración).
         
         ## Instalación
         
         [nacal](https://pypi.org/project/nacal/) funciona con Python \>=3.6.
         Puede instalar el paquete desde PyPI via pip:
```

### Comparing `nacal-0.2.0/README.md` & `nacal-0.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
-[\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)\]\]
+[![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)
+[![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
 
 # Módulo "NAcAL" (Notación Asociativa para un Curso de Álgebra Lineal)
 
 Este módulo implementa la notación, los objetos y los procedimientos
 descritos en el
 [libro](https://mbujosab.github.io/CursoDeAlgebraLineal/libro.pdf) del
 [Curso de ÁLgebra
 Lineal](https://github.com/mbujosab/CursoDeAlgebraLineal)
 correspondiente a la asignatura [Matemáticas
 II.](https://www.ucm.es/fundamentos-analisis-economico2/algebra-2)
 
 Aunque es posible su uso desde un terminal, este módulo está pensado
 para ser empleado en [Notebooks de Jupyter](https://jupyter.org/) (y
-también desde documentos de \(\LaTeX{}\)).
+también desde documentos de LaTeX).
 
 Este módulo muestra cómo llegar a la mayoría de los resultados del curso
 de Álgebra Lineal empleando el método de eliminación. NAcAL no solo
 resuelve sistemas de ecuaciones, invierte matrices, calcula
 determinantes, diagonaliza matrices tanto por semejanza como por
 congruencia, etc. sino que muestra los pasos empleados para llegar al
 resultado como si se hiciera con lápiz y papel (ofreciendo el código
@@ -31,15 +31,15 @@
 La documentación explica la programación del código y sirve como
 material adicional al [libro del
 curso](https://github.com/mbujosab/CursoDeAlgebraLineal) (este módulo es
 una implementación literal de lo mostrado en dicho libro).
 
 Puede ver el uso del módulo sin necesidad de instalar nada, tan solo
 accediendo a los Notebooks de Jupyter alojados en
-[\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
+[![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
 con su navegador de páginas web (tenga en cuenta que MyBinder puede
 tardar unos minutos en cargar el módulo y el Notebook de demostración).
 
 ## Instalación
 
 [nacal](https://pypi.org/project/nacal/) funciona con Python \>=3.6.
 Puede instalar el paquete desde PyPI via pip:
```

### Comparing `nacal-0.2.0/nacal/nacal.py` & `nacal-0.2.1/nacal/nacal.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,19 +375,26 @@
                     lista += [item]
             return lista
         
         return BlockV(vectoriza(self))
     
     def subs(self, reglasDeSustitucion=[]):
         """ Sustitución de variables simbólicas """
+        
+        def sustitucion(elemento, regla_de_sustitucion):
+            if es_numero(elemento):
+                return sympy.S(elemento).subs(CreaLista(regla_de_sustitucion))
+            else:
+                return elemento.subs(CreaLista(regla_de_sustitucion))
+            
         reglas = CreaLista(reglasDeSustitucion)
         NuevoSistema = self.fullcopy()
-        NuevoSistema.lista = [sympy.S(elemento).subs(CreaLista(reglas)) for elemento in NuevoSistema]
+        NuevoSistema.lista = [sustitucion(elemento, reglasDeSustitucion) for elemento in NuevoSistema]
         return NuevoSistema
-    
+        
     
     def simplify(self):
         """ Simplificación de expresiones simbólicas """
         self.lista = [simplify(elemento) for elemento in self.lista]
                                                                    
     def factor(self):
         """ Factorización de expresiones simbólicas """
@@ -1937,14 +1944,106 @@
 
 class I(Matrix):
     def __init__(self, n):
         """ Inicializa la matriz identidad de tamaño n """
         super().__init__([[(i==j)*1 for i in range(n)] for j in range(n)])
         self.__class__ = Matrix
 
+class SistemaSimbol(BlockV):
+    def __init__(self, arg, char=' ', rpr='columna'):
+        """Inicializa un Sistema Simbólico con una lista, tupla o Sistema"""
+        self.sistema = arg if isinstance(arg, Sistema) else Sistema(CreaLista(arg))
+        letra, simbolo = self.simbolos(char)        
+        self.lista   = [self.sistema, simbolo, letra]
+        
+        self.n = len(self.sistema)
+        self.corteSistema = set()
+        self.rpr = rpr
+                            
+    def simbolos(self, char):
+        letra = sympy.Symbol('0', zero=True) if self.es_nulo() else sympy.Symbol(char.upper())
+        simbolo_latex = sympy.Symbol(r'\mathsf{0}', zero=True) if self.es_nulo() else  sympy.Symbol(r'\mathsf{'+str(letra)+'}')
+        return letra, simbolo_latex
+    
+    def es_nulo(self):
+        return self.sistema.es_nulo()
+    
+    def copy(self):
+        """ Genera una copia de un SistemaSimbol """
+        return type(self)(self.lista[0], str(self.lista[2]))
+
+    def __str__(self):
+        """ Muestra un SistemaSimbol en su representación python """
+        return str(self.lista[2])
+    
+    def __repr__(self):
+        """ Muestra un SistemaSimbol en su representación python """
+        return 'SistemaSimbol(' + repr(self.lista[0]) + ', "' + repr(self.lista[2]) + '")'
+    
+    def latex(self):
+        """ Construye el comando LaTeX para representar un SistemaSimbol """
+        return latex(self.lista[1])
+        
+    def _repr_latex_(self):
+        """ Representación para el entorno jupyter en Emacs """
+        return '$'+self.latex()+'$'
+    
+    def _repr_html_(self):
+        """ Construye la representación para el entorno jupyter notebook """
+        return html(self.latex())
+
+    def elim(self, variante=0, rep=False, sust=[], repsust=False):
+        return self.sistema.elim(variante, rep, sust, repsust)
+    
+class MatrixSimbol(SistemaSimbol):
+    def __init__(self, arg, char=' ', rpr='columna'):
+        self.sistema = arg if isinstance(arg, Matrix) else BlockM(CreaLista(arg))
+        letra, simbolo = self.simbolos(char)        
+        self.lista   = [self.sistema, simbolo, letra]
+        
+        self.n = len(self.sistema)
+        self.corteSistema = set()
+        self.rpr = rpr
+                            
+    def simbolos(self, char):
+        letra = sympy.Symbol('0', zero=True) if self.es_nulo() else sympy.Symbol(char.upper())
+        simbolo_latex = sympy.Symbol(r'\boldsymbol{\mathsf{0}}', zero=True) if self.es_nulo() else  sympy.Symbol(r'\boldsymbol{\mathsf{'+str(letra)+'}}')
+        return letra, simbolo_latex
+    
+    def __repr__(self):
+        """ Muestra un MatrixSimbol en su representación python """
+        return 'MatrixSimbol(' + repr(self.lista[0]) + ', "' + repr(self.lista[2]) + '")'
+    
+    def latex(self):
+        """ Construye el comando LaTeX para representar un MatrixSimbol """
+        return latex(self.lista[1])
+    
+class VectorSimbol(SistemaSimbol):
+    def __init__(self, arg, char=' ', rpr='columna'):
+        self.sistema = arg if isinstance(arg, Vector) else BlockV(CreaLista(arg))
+        letra, simbolo = self.simbolos(char)
+        self.lista   = [self.sistema, simbolo, letra]
+        
+        self.n = len(self.sistema)
+        self.corteSistema = set()
+        self.rpr = rpr
+                            
+    def simbolos(self, char):
+        letra = sympy.Symbol('0', zero=True) if self.es_nulo() else sympy.Symbol(char.lower())
+        simbolo_latex = sympy.Symbol(r'\boldsymbol{0}', zero=True) if self.es_nulo() else  sympy.Symbol(r'\boldsymbol{'+str(letra)+'}')
+        return letra, simbolo_latex
+
+    def __repr__(self):
+        """ Muestra un VectorSimbol en su representación python """
+        return 'VectorSimbol(' + repr(self.lista[0]) + ', "' + repr(self.lista[2]) + '")'
+    
+    def latex(self):
+        """ Construye el comando LaTeX para representar un VectorSimbol """
+        return latex(self.lista[1])
+    
 
 RistraTypes = (tuple, list, Sistema)
 es_ristra  = lambda x: isinstance(x, RistraTypes) 
 
 def es_ristra_de_numeros(arg):
     return all( [es_numero(elemento) for elemento in arg] ) if es_ristra(arg) else None
```

### Comparing `nacal-0.2.0/nacal.egg-info/PKG-INFO` & `nacal-0.2.1/nacal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: nacal
-Version: 0.2.0
+Version: 0.2.1
 Summary: Notacion Asociativa para un curso de Algebra Lineal (NAcAL)
 Home-page: https://github.com/mbujosab/nacallib
 Author: Marcos Bujosa
 Author-email: mbujosab@ucm.es
 License: GPLv3
-Description: [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
-        [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)\]\]
+Description: [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)
+        [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
         
         # Módulo "NAcAL" (Notación Asociativa para un Curso de Álgebra Lineal)
         
         Este módulo implementa la notación, los objetos y los procedimientos
         descritos en el
         [libro](https://mbujosab.github.io/CursoDeAlgebraLineal/libro.pdf) del
         [Curso de ÁLgebra
         Lineal](https://github.com/mbujosab/CursoDeAlgebraLineal)
         correspondiente a la asignatura [Matemáticas
         II.](https://www.ucm.es/fundamentos-analisis-economico2/algebra-2)
         
         Aunque es posible su uso desde un terminal, este módulo está pensado
         para ser empleado en [Notebooks de Jupyter](https://jupyter.org/) (y
-        también desde documentos de \(\LaTeX{}\)).
+        también desde documentos de LaTeX).
         
         Este módulo muestra cómo llegar a la mayoría de los resultados del curso
         de Álgebra Lineal empleando el método de eliminación. NAcAL no solo
         resuelve sistemas de ecuaciones, invierte matrices, calcula
         determinantes, diagonaliza matrices tanto por semejanza como por
         congruencia, etc. sino que muestra los pasos empleados para llegar al
         resultado como si se hiciera con lápiz y papel (ofreciendo el código
@@ -39,15 +39,15 @@
         La documentación explica la programación del código y sirve como
         material adicional al [libro del
         curso](https://github.com/mbujosab/CursoDeAlgebraLineal) (este módulo es
         una implementación literal de lo mostrado en dicho libro).
         
         Puede ver el uso del módulo sin necesidad de instalar nada, tan solo
         accediendo a los Notebooks de Jupyter alojados en
-        [\[\[<https://mybinder.org/badge_logo.svg>](https://mybinder.org/v2/gh/mbujosab/nacallib/master?filepath=doc%2FNotebooks%2FNotebook.ipynb)\]\]
+        [![](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mbujosab/nacal-Jupyter-Notebooks/master)
         con su navegador de páginas web (tenga en cuenta que MyBinder puede
         tardar unos minutos en cargar el módulo y el Notebook de demostración).
         
         ## Instalación
         
         [nacal](https://pypi.org/project/nacal/) funciona con Python \>=3.6.
         Puede instalar el paquete desde PyPI via pip:
```

### Comparing `nacal-0.2.0/setup.py` & `nacal-0.2.1/setup.py`

 * *Files identical despite different names*

