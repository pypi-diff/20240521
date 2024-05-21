# Comparing `tmp/stencila_types-2.0.0a28.tar.gz` & `tmp/stencila_types-2.0.0a29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stencila_types-2.0.0a28.tar", last modified: Mon Mar 25 10:05:34 2024, max compression
+gzip compressed data, was "stencila_types-2.0.0a29.tar", last modified: Tue May 21 01:55:23 2024, max compression
```

## Comparing `stencila_types-2.0.0a28.tar` & `stencila_types-2.0.0a29.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2734 2024-03-25 10:01:43.672040 stencila_types-2.0.0a28/README.md
--rw-r--r--   0        0        0     1996 2024-03-25 10:05:34.314228 stencila_types-2.0.0a28/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-25 05:10:28.068087 stencila_types-2.0.0a28/src/stencila_types/__init__.py
--rw-r--r--   0        0        0     8619 2024-03-25 05:11:24.680034 stencila_types-2.0.0a28/src/stencila_types/shortcuts.py
--rw-r--r--   0        0        0    75568 2024-03-25 08:33:33.449105 stencila_types-2.0.0a28/src/stencila_types/types.py
--rw-r--r--   0        0        0     1937 2024-03-25 05:11:09.308105 stencila_types-2.0.0a28/src/stencila_types/utilities.py
--rw-r--r--   0        0        0        0 2024-03-25 05:10:28.068681 stencila_types-2.0.0a28/tests/__init__.py
--rw-r--r--   0        0        0      917 2024-03-25 05:10:59.326315 stencila_types-2.0.0a28/tests/conftest.py
--rw-r--r--   0        0        0     1280 2024-03-25 05:10:59.350028 stencila_types-2.0.0a28/tests/test_shortcuts.py
--rw-r--r--   0        0        0       73 2024-03-25 05:10:59.350142 stencila_types-2.0.0a28/tests/test_shortcuts/test_emphasis.yml
--rw-r--r--   0        0        0      120 2024-03-25 05:10:59.350206 stencila_types-2.0.0a28/tests/test_shortcuts/test_link.yml
--rw-r--r--   0        0        0      104 2024-03-25 05:10:59.350260 stencila_types-2.0.0a28/tests/test_shortcuts/test_quote.yml
--rw-r--r--   0        0        0      399 2024-03-25 05:10:59.326431 stencila_types-2.0.0a28/tests/test_types.py
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 stencila_types-2.0.0a28/PKG-INFO
+-rw-r--r--   0        0        0     2734 2024-03-26 01:26:24.324834 stencila_types-2.0.0a29/README.md
+-rw-r--r--   0        0        0     1996 2024-05-21 01:55:23.263989 stencila_types-2.0.0a29/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-26 01:26:24.325553 stencila_types-2.0.0a29/src/stencila_types/__init__.py
+-rw-r--r--   0        0        0     8619 2024-04-02 00:34:19.791089 stencila_types-2.0.0a29/src/stencila_types/shortcuts.py
+-rw-r--r--   0        0        0    78959 2024-05-21 00:24:17.661749 stencila_types-2.0.0a29/src/stencila_types/types.py
+-rw-r--r--   0        0        0     1937 2024-05-20 23:13:11.800836 stencila_types-2.0.0a29/src/stencila_types/utilities.py
+-rw-r--r--   0        0        0        0 2024-03-26 01:26:24.326808 stencila_types-2.0.0a29/tests/__init__.py
+-rw-r--r--   0        0        0      917 2024-03-26 01:26:24.327098 stencila_types-2.0.0a29/tests/conftest.py
+-rw-r--r--   0        0        0     1280 2024-03-26 01:26:24.327180 stencila_types-2.0.0a29/tests/test_shortcuts.py
+-rw-r--r--   0        0        0       73 2024-03-26 01:26:24.327296 stencila_types-2.0.0a29/tests/test_shortcuts/test_emphasis.yml
+-rw-r--r--   0        0        0      120 2024-03-26 01:26:24.327362 stencila_types-2.0.0a29/tests/test_shortcuts/test_link.yml
+-rw-r--r--   0        0        0      104 2024-03-26 01:26:24.327422 stencila_types-2.0.0a29/tests/test_shortcuts/test_quote.yml
+-rw-r--r--   0        0        0      399 2024-05-20 23:13:11.800996 stencila_types-2.0.0a29/tests/test_types.py
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 stencila_types-2.0.0a29/PKG-INFO
```

### Comparing `stencila_types-2.0.0a28/README.md` & `stencila_types-2.0.0a29/README.md`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a28/pyproject.toml` & `stencila_types-2.0.0a29/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stencila_types"
-version = "2.0.0a28"
+version = "2.0.0a29"
 description = "Python types for Stencila"
 readme = "README.md"
 authors = [
     { name = "Nokome Bentley", email = "nokome@stencila.io" },
 ]
 dependencies = [
     "cattrs>=23.2.3",
```

### Comparing `stencila_types-2.0.0a28/src/stencila_types/shortcuts.py` & `stencila_types-2.0.0a29/src/stencila_types/shortcuts.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a28/src/stencila_types/types.py` & `stencila_types-2.0.0a29/src/stencila_types/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 
 
 class AuthorRoleName(StrEnum):
     """
     A `roleName` for an `AuthorRole`.
     """
 
+    Importer = "Importer"
     Writer = "Writer"
     Verifier = "Verifier"
     Instructor = "Instructor"
     Prompter = "Prompter"
     Generator = "Generator"
 
 
@@ -320,14 +321,38 @@
     """
 
     Footnote = "Footnote"
     Endnote = "Endnote"
     Sidenote = "Sidenote"
 
 
+class ProvenanceCategory(StrEnum):
+    """
+    A description of the provenance of content in terms of human/machine involvement.
+    """
+
+    HwHeHv = "HwHeHv"
+    HwHe = "HwHe"
+    HwHv = "HwHv"
+    Hw = "Hw"
+    HwMv = "HwMv"
+    MwHeHv = "MwHeHv"
+    MwHe = "MwHe"
+    MwHeMv = "MwHeMv"
+    HwMeHv = "HwMeHv"
+    HwMe = "HwMe"
+    HwMeMv = "HwMeMv"
+    MwHv = "MwHv"
+    MwMeHv = "MwMeHv"
+    Mw = "Mw"
+    MwMv = "MwMv"
+    MwMe = "MwMe"
+    MwMeMv = "MwMeMv"
+
+
 class SectionType(StrEnum):
     """
     The type of a `Section`.
     """
 
     Main = "Main"
     Header = "Header"
@@ -443,14 +468,17 @@
 
     abstract: list[Block] | None = None
     """A a short description that summarizes a `CreativeWork`."""
 
     authors: list[Author] | None = None
     """The authors of the `CreativeWork`."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the work."""
+
     contributors: list[Author] | None = None
     """A secondary contributor to the `CreativeWork`."""
 
     editors: list[Person] | None = None
     """People who edited the `CreativeWork`."""
 
     maintainers: list[Person | Organization] | None = None
@@ -587,14 +615,17 @@
 
     programming_language: str | None = None
     """The programming language of the code."""
 
     authors: list[Author] | None = None
     """The authors of the executable code."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the code."""
+
 
 @dataclass(kw_only=True, repr=False)
 class CodeStatic(Entity):
     """
     Abstract base type for non-executable code nodes (e.g. `CodeBlock`).
     """
 
@@ -605,14 +636,17 @@
 
     programming_language: str | None = None
     """The programming language of the code."""
 
     authors: list[Author] | None = None
     """The authors of the code."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the code."""
+
 
 @dataclass(kw_only=True, repr=False)
 class ContactPoint(Thing):
     """
     A contact point, usually within an organization.
     """
 
@@ -671,23 +705,23 @@
     """
 
     type: Literal["Instruction"] = "Instruction"
 
     messages: list[InstructionMessage]
     """Messages involved in the instruction."""
 
-    candidates: list[str] | None = None
-    """A list of candidates for the assignee property."""
-
     assignee: str | None = None
     """An identifier for the agent assigned to perform the instruction"""
 
     authors: list[Author] | None = None
     """The authors of the instruction."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the messages and content within the instruction."""
+
 
 @dataclass(kw_only=True, repr=False)
 class Mark(Entity):
     """
     Abstract base class for nodes that mark some other inline content in some way (e.g. as being emphasised, or quoted).
     """
 
@@ -710,14 +744,17 @@
 
     math_language: str | None = None
     """The language used for the equation e.g tex, mathml, asciimath."""
 
     authors: list[Author] | None = None
     """The authors of the math."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the math."""
+
     compilation_digest: CompilationDigest | None = None
     """A digest of the `code` and `mathLanguage`."""
 
     compilation_messages: list[CompilationMessage] | None = None
     """Messages generated while parsing and compiling the math expression."""
 
     mathml: str | None = None
@@ -819,15 +856,18 @@
     code: Cord
     """The code of the equation in the `styleLanguage`."""
 
     style_language: str | None = None
     """The language used for the style specification e.g. css, tw"""
 
     authors: list[Author] | None = None
-    """The authors of the styling code."""
+    """The authors of the code and content in the styled node."""
+
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the code and content in the styed node."""
 
     compilation_digest: CompilationDigest | None = None
     """A digest of the `code` and `styleLanguage`."""
 
     compilation_messages: list[CompilationMessage] | None = None
     """Messages generated while parsing and transpiling the style."""
 
@@ -881,14 +921,17 @@
 
     content: list[Block]
     """The content within the section."""
 
     authors: list[Author] | None = None
     """The authors of the admonition."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the admonition."""
+
 
 @dataclass(kw_only=True, repr=False)
 class ArrayHint(Entity):
     """
     A hint to the content of an `Array`.
     """
 
@@ -977,22 +1020,25 @@
 class AuthorRole(Role):
     """
     An author and their role.
     """
 
     type: Literal["AuthorRole"] = "AuthorRole"
 
-    author: Person | Organization | SoftwareApplication
-    """The author."""
+    author: AuthorRoleAuthor
+    """The entity acting as an author."""
 
     role_name: AuthorRoleName
-    """A role played by the author."""
+    """The role played by the author."""
+
+    format: str | None = None
+    """The format that the author used to perform the role. e.g. Markdown, Python"""
 
     last_modified: Timestamp | None = None
-    """Timestamp of most recent modification by the author in the role."""
+    """Timestamp of most recent modification, by the author, in the role."""
 
 
 @dataclass(kw_only=True, repr=False)
 class BooleanValidator(Entity):
     """
     A schema specifying that a node must be a boolean value.
     """
@@ -1037,14 +1083,17 @@
 class CallArgument(Parameter):
     """
     The value of a `Parameter` to call a document with.
     """
 
     type: Literal["CallArgument"] = "CallArgument"
 
+    value: Node | None = None
+    """The current value of the argument."""
+
     code: Cord
     """The code to be evaluated for the parameter."""
 
     programming_language: str | None = None
     """The programming language of the code."""
 
 
@@ -1145,20 +1194,26 @@
 
     label_type: LabelType | None = None
     """The type of the label for the chunk."""
 
     label: str | None = None
     """A short label for the chunk."""
 
+    label_automatically: bool | None = None
+    """Whether the label should be automatically updated."""
+
     caption: list[Block] | None = None
     """A caption for the chunk."""
 
     outputs: list[Node] | None = None
     """Outputs from executing the chunk."""
 
+    is_invisible: bool | None = None
+    """Whether the outputs of the code chunk should be invisible to the reader."""
+
     execution_pure: bool | None = None
     """Whether the code should be treated as side-effect free when executed."""
 
 
 @dataclass(kw_only=True, repr=False)
 class CodeExpression(CodeExecutable):
     """
@@ -1610,14 +1665,17 @@
 
     content: list[Block]
     """The content of the figure."""
 
     label: str | None = None
     """A short label for the figure."""
 
+    label_automatically: bool | None = None
+    """Whether the label should be automatically updated."""
+
     caption: list[Block] | None = None
     """A caption for the figure."""
 
 
 @dataclass(kw_only=True, repr=False)
 class File(Entity):
     """
@@ -1649,15 +1707,15 @@
 
     content: list[Block]
     """The content to repeat for each item"""
 
     otherwise: list[Block] | None = None
     """The content to render if there are no items"""
 
-    iterations: list[Section] | None = None
+    iterations: list[Block] | None = None
     """The content repeated for each iteration"""
 
 
 @dataclass(kw_only=True, repr=False)
 class Form(Executable):
     """
     A form to batch updates in document parameters.
@@ -1709,29 +1767,29 @@
 
     content: list[Inline]
     """Content of the heading."""
 
     authors: list[Author] | None = None
     """The authors of the heading."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the heading."""
+
 
 @dataclass(kw_only=True, repr=False)
 class IfBlock(Executable):
     """
     Show and execute alternative content conditional upon an executed expression.
     """
 
     type: Literal["IfBlock"] = "IfBlock"
 
     clauses: list[IfBlockClause]
     """The clauses making up the `IfBlock` node"""
 
-    authors: list[Author] | None = None
-    """The authors of the if block."""
-
 
 @dataclass(kw_only=True, repr=False)
 class IfBlockClause(CodeExecutable):
     """
     A clause within an `IfBlock` node.
     """
 
@@ -1871,14 +1929,17 @@
 
     order: ListOrder
     """The ordering of the list."""
 
     authors: list[Author] | None = None
     """The authors of the list."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the list."""
+
 
 @dataclass(kw_only=True, repr=False)
 class ListItem(Thing):
     """
     A single item in a list.
     """
 
@@ -1904,14 +1965,17 @@
     """
 
     type: Literal["MathBlock"] = "MathBlock"
 
     label: str | None = None
     """A short label for the math block."""
 
+    label_automatically: bool | None = None
+    """Whether the label should be automatically updated."""
+
 
 @dataclass(kw_only=True, repr=False)
 class MathInline(Math):
     """
     A fragment of math, e.g a variable name, to be treated as inline content.
     """
 
@@ -2051,14 +2115,17 @@
 
     content: list[Inline]
     """The contents of the paragraph."""
 
     authors: list[Author] | None = None
     """The authors of the paragraph."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of content within the paragraph."""
+
 
 @dataclass(kw_only=True, repr=False)
 class Periodical(CreativeWork):
     """
     A periodical publication.
     """
 
@@ -2173,14 +2240,32 @@
     """A commonly used identifier for the characteristic represented by the property."""
 
     value: Primitive
     """The value of the property."""
 
 
 @dataclass(kw_only=True, repr=False)
+class ProvenanceCount(Entity):
+    """
+    The count of the number of characters in a `ProvenanceCategory` within an entity.
+    """
+
+    type: Literal["ProvenanceCount"] = "ProvenanceCount"
+
+    provenance_category: ProvenanceCategory
+    """The provenance category that the character count applies to."""
+
+    character_count: UnsignedInteger
+    """The number of characters in the provenance category."""
+
+    character_percent: UnsignedInteger | None = None
+    """The percentage of characters in the provenance category."""
+
+
+@dataclass(kw_only=True, repr=False)
 class PublicationIssue(CreativeWork):
     """
     A part of a successively published publication such as a periodical or publication volume, often numbered.
     """
 
     type: Literal["PublicationIssue"] = "PublicationIssue"
 
@@ -2231,14 +2316,17 @@
 
     content: list[Block]
     """The content of the quote."""
 
     authors: list[Author] | None = None
     """The authors of the quote."""
 
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the section."""
+
 
 @dataclass(kw_only=True, repr=False)
 class QuoteInline(Mark):
     """
     Inline, quoted content.
     """
 
@@ -2297,14 +2385,20 @@
 
     content: list[Block]
     """The content within the section."""
 
     section_type: SectionType | None = None
     """The type of section."""
 
+    authors: list[Author] | None = None
+    """The authors of the section."""
+
+    provenance: list[ProvenanceCount] | None = None
+    """A summary of the provenance of the content within the section."""
+
 
 @dataclass(kw_only=True, repr=False)
 class SoftwareApplication(CreativeWork):
     """
     A software application.
     """
 
@@ -2474,14 +2568,17 @@
     """
 
     type: Literal["Table"] = "Table"
 
     label: str | None = None
     """A short label for the table."""
 
+    label_automatically: bool | None = None
+    """Whether the label should be automatically updated."""
+
     caption: list[Block] | None = None
     """A caption for the table."""
 
     rows: list[TableRow]
     """Rows of cells in the table."""
 
     notes: list[Block] | None = None
@@ -2692,14 +2789,25 @@
     AuthorRole,
 ]
 """
 Union type for things that can be an author of a `CreativeWork` or other type.
 """
 
 
+AuthorRoleAuthor = Union[
+    Person,
+    Organization,
+    SoftwareApplication,
+    Thing,
+]
+"""
+Union type for things that can be an author in `AuthorRole`.
+"""
+
+
 Block = Union[
     Admonition,
     CallBlock,
     Claim,
     CodeBlock,
     CodeChunk,
     DeleteBlock,
@@ -2942,14 +3050,15 @@
     Paragraph,
     Parameter,
     Periodical,
     Person,
     PostalAddress,
     Product,
     PropertyValue,
+    ProvenanceCount,
     PublicationIssue,
     PublicationVolume,
     QuoteBlock,
     QuoteInline,
     ReplaceBlock,
     ReplaceInline,
     Review,
@@ -3045,14 +3154,15 @@
     NoteType,
     Organization,
     Periodical,
     Person,
     PostalAddress,
     Product,
     PropertyValue,
+    ProvenanceCategory,
     PublicationIssue,
     PublicationVolume,
     Review,
     SectionType,
     SoftwareApplication,
     SoftwareSourceCode,
     SuggestionStatus,
```

### Comparing `stencila_types-2.0.0a28/src/stencila_types/utilities.py` & `stencila_types-2.0.0a29/src/stencila_types/utilities.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a28/tests/conftest.py` & `stencila_types-2.0.0a29/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a28/tests/test_shortcuts.py` & `stencila_types-2.0.0a29/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `stencila_types-2.0.0a28/PKG-INFO` & `stencila_types-2.0.0a29/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: stencila_types
-Version: 2.0.0a28
+Version: 2.0.0a29
 Summary: Python types for Stencila
-Keywords: programmable reproducible interactive documents python SDK
+Keywords: programmable,reproducible,interactive,documents,python,SDK
 Author-Email: Nokome Bentley <nokome@stencila.io>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Software Development
```

