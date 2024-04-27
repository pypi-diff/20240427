# Comparing `tmp/bbm25_haystack-0.2.0.tar.gz` & `tmp/bbm25_haystack-0.2.1.tar.gz`

## Comparing `bbm25_haystack-0.2.0.tar` & `bbm25_haystack-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,26 @@
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/benchmarks/.gitkeep
--rw-r--r--   0        0        0     7092 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/scripts/benchmark_beir.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/__about__.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/__init__.py
--rw-r--r--   0        0        0     5124 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_retriever.py
--rw-r--r--   0        0        0    13984 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_store.py
--rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/default.model
--rw-r--r--   0        0        0     8512 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/src/bbm25_haystack/filters.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/test_document_store.py
--rw-r--r--   0        0        0     7623 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/tests/test_retriever.py
--rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/LICENSE
--rw-r--r--   0        0        0     5535 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/README.md
--rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/.github/workflows/test.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/benchmarks/.gitkeep
+-rw-r--r--   0        0        0   265513 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/bbm25_haystack.html
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/index.html
+-rw-r--r--   0        0        0   115822 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/search.js
+-rw-r--r--   0        0        0    35785 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/bbm25_haystack/__about__.html
+-rw-r--r--   0        0        0   129529 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/bbm25_haystack/bbm25_retriever.html
+-rw-r--r--   0        0        0   282581 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/bbm25_haystack/bbm25_store.html
+-rw-r--r--   0        0        0    93054 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/docs/bbm25_haystack/filters.html
+-rw-r--r--   0        0        0     7311 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/scripts/benchmark_beir.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/__about__.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/__init__.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/bbm25_retriever.py
+-rw-r--r--   0        0        0    14175 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/bbm25_store.py
+-rw-r--r--   0        0        0   499723 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/default.model
+-rw-r--r--   0        0        0     9038 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/src/bbm25_haystack/filters.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     6079 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/tests/test_document_store.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/tests/test_retriever.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/LICENSE
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/README.md
+-rw-r--r--   0        0        0     3622 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7388 2020-02-02 00:00:00.000000 bbm25_haystack-0.2.1/PKG-INFO
```

### Comparing `bbm25_haystack-0.2.0/.github/workflows/test.yml` & `bbm25_haystack-0.2.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/scripts/benchmark_beir.py` & `bbm25_haystack-0.2.1/scripts/benchmark_beir.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,15 @@
         dir_raw = DIR_BEIR_RAW / ds_name
 
         store = BetterBM25DocumentStore(
             k=args.bm25_k1,
             b=args.bm25_b,
             delta=args.bm25_delta,
             sp_file=args.sp_file,
+            n_grams=args.n_grams,
         )
         model = BEIRWrapper(store)
         retriever = EvaluateRetrieval(model)
 
         corpus, queries, qrels = GenericDataLoader(dir_raw).load(split=args.split)
         results = retriever.retrieve(corpus, queries)
 
@@ -218,14 +219,21 @@
         "--sp-file",
         type=str,
         default=None,
         required=False,
         help="Path to the SentencePiece model file; default to None (LLaMA2)",
     )
     parser.add_argument(
+        "--n-grams",
+        type=int,
+        default=1,
+        required=False,
+        help="The n-gram size up to n for tokenizations; default to 1",
+    )
+    parser.add_argument(
         "--split",
         type=str,
         default="test",
         required=False,
         choices=["train", "dev", "test"],
         help="Dataset split to evaluate on (default: 'test')",
     )
```

### Comparing `bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_retriever.py` & `bbm25_haystack-0.2.1/src/bbm25_haystack/bbm25_retriever.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,102 +14,113 @@
 from bbm25_haystack.bbm25_store import BetterBM25DocumentStore
 
 
 def _validate_search_params(filters: Optional[dict[str, Any]], top_k: int) -> None:
     """
     Validate the search parameters.
 
-    :param filters: A dictionary with filters to narrow down the search space
-        (default is None).
-    :type filters: Optional[dict[str, Any]]
-    :param top_k: The maximum number of documents to retrieve (default is 10).
-    :type top_k: int
+    :param filters: Haystack filters, a dictionary with filters to
+        narrow down the search space. The filters are applied
+        **before** similarity retrieval.
+    :type filters: ``Optional[dict[str, Any]]``
+    :param top_k: The maximum number of documents to return.
+    :type top_k: ``int``
 
     :raises ValueError: If the specified top_k is not > 0.
     :raises TypeError: If filters is not a dictionary.
     """
     if not isinstance(top_k, int):
-        msg = f"top_k must be an integer; got {type(top_k)} instead"
+        msg = f"top_k must be an integer; got {type(top_k)} instead."
         raise TypeError(msg)
 
     if top_k <= 0:
-        msg = f"top_k must be > 0; got {top_k} instead"
+        msg = f"top_k must be > 0; got {top_k} instead."
         raise ValueError(msg)
 
     if filters is not None and (not isinstance(filters, dict)):
-        msg = f"filters must be a dictionary; got {type(filters)} instead"
+        msg = f"filters must be a dictionary; got {type(filters)} instead."
         raise TypeError(msg)
 
 
 @component
 class BetterBM25Retriever:
     """
-    A component for retrieving documents from an BetterBM25DocumentStore.
+    A component for retrieving documents from a ``BetterBM25DocumentStore``.
     """
 
     def __init__(
         self,
         document_store: BetterBM25DocumentStore,
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: int = 10,
         set_score: bool = True,
     ) -> None:
         """
-        Create an BetterBM25Retriever component.
+        Create a ``BetterBM25Retriever`` component.
 
-        :param document_store: A Document Store object used to
-            retrieve documents
-        :type document_store: BetterBM25DocumentStore
-        :param filters: A dictionary with filters to narrow down the
-            search space (default is None).
-        :type filters: Optional[dict[str, Any]]
-        :param top_k: The maximum number of documents to retrieve
-            (default is 10).
-        :type top_k: int
-        :param set_score: Whether to set the similarity scores
-            to retrieved documents (default is True).
-        :type set_score: bool
-
-        :raises ValueError: If the specified top_k is not > 0.
+        :param document_store: A ``BetterBM25DocumentStore`` instance.
+        :type document_store: ``BetterBM25DocumentStore``
+        :param filters: Haystack filters, a dictionary with filters to
+            narrow down the search space. The filters are applied
+            **before** similarity retrieval.
+        :type filters: ``Optional[dict[str, Any]]``
+        :param top_k: The maximum number of documents to return.
+        :type top_k: ``int``
+        :param set_score: Whether to set the similarity scores to returned
+            documents under ``Document.score`` attribute. This is useful in
+            hybrid retrieval setting where you may want to merge results.
+            Note that returned documents are **copies** so that the original
+            instances in the document store are not modified.
+        :type set_score: ``bool``
+
+        :raises ValueError: If the ``filters`` or ``top_k`` is invalid.
+        :raises TypeError: If the ``document_store`` is not an instance of
+            ``BetterBM25DocumentStore``.
         """
         _validate_search_params(filters, top_k)
 
         self.filters = filters
+        """@private"""
+
         self.top_k = top_k
+        """@private"""
+
         self.set_score = set_score
+        """@private"""
 
         if not isinstance(document_store, BetterBM25DocumentStore):
-            msg = "document_store must be an instance of BetterBM25DocumentStore"
+            msg = "'document_store' must be of type 'BetterBM25DocumentStore'"
             raise TypeError(msg)
+
         self.document_store = document_store
+        """@private"""
 
     @component.output_types(documents=list[Document])
     def run(
         self,
         query: str,
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: Optional[int] = None,
     ) -> dict[str, list[Document]]:
         """
-        Run the Retriever on the given query.
-
-        This method always return copies of the documents
-        retrieved from the document store.
+        Run the Retriever on the given query. This method always return
+        copies of the documents retrieved from the document store.
 
-        :param query: The query to run the Retriever on.
-        :type query: str
-        :param filters: A dictionary with filters to narrow
-            down the search space (default is None).
-        :type filters: Optional[dict[str, Any]]
-        :param top_k: The maximum number of documents to
-            retrieve (default is None).
+        :param query: The text search term.
+        :type query: ``str``
+        :param filters: Haystack filters, a dictionary with filters to
+            narrow down the search space. The filters are applied
+            **before** similarity retrieval.
+        :type filters: ``Optional[dict[str, Any]]``
+        :param top_k: The maximum number of documents to return.
+        :type top_k: ``Optional[int]``
 
-        :return: The retrieved documents.
+        :return: The retrieved documents in a dictionary with key "documents".
         """
         filters = filters or self.filters
         top_k = top_k or self.top_k
 
         _validate_search_params(filters, top_k)
 
         sim = self.document_store._retrieval(query, filters=filters, top_k=top_k)
@@ -120,35 +131,26 @@
             if self.set_score:
                 data["score"] = scr
             ret.append(Document.from_dict(data))
 
         return {"documents": ret}
 
     def to_dict(self) -> dict[str, Any]:
-        """
-        Serializes the component to a dictionary.
-
-        :return: dictionary with serialized data.
-        """
+        """Serializes the component to a dictionary."""
         return default_to_dict(
             self,
             filters=self.filters,
             top_k=self.top_k,
             document_store=self.document_store.to_dict(),
             set_score=self.set_score,
         )
 
     @classmethod
     def from_dict(cls, data: dict[str, Any]) -> "BetterBM25Retriever":
-        """
-        Deserializes the component from a dictionary.
-
-        :param data: dictionary to deserialize from.
-        :returns: deserialized component.
-        """
+        """Deserializes the retriever from a dictionary."""
         doc_store_params = data["init_parameters"].get("document_store")
         if doc_store_params is None:
             msg = "Missing 'document_store' in serialization data"
             raise DeserializationError(msg)
 
         if doc_store_params.get("type") is None:
             msg = "Missing 'type' in document store's serialization data"
```

### Comparing `bbm25_haystack-0.2.0/src/bbm25_haystack/bbm25_store.py` & `bbm25_haystack-0.2.1/src/bbm25_haystack/bbm25_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,90 +22,90 @@
 from bbm25_haystack.filters import apply_filters_to_document
 
 logger = logging.getLogger(__name__)
 
 
 def _n_grams(seq: Iterable[str], n: int):
     """
-    Returns a sliding window (of width n) over data from the iterable.
+    Returns a sliding window (of width n) over data from the
+    iterable. This solution is adapted from the StackOverflow
+    answer [here](https://stackoverflow.com/a/6822773/13403958).
+
+    :param seq: Input token sequence.
+    :type seq: ``Iterable[str]``
+    :param n: Window size.
+    :type n: ``int``
 
-    :param seq: the input token sequence.
-    :type seq: Iterable[str]
-    :param n: the window size.
-    :type n: int
-
-    :return: the n-gram window generator.
-    :rtype: Generator[tuple[str], None, None]
+    :return: The n-gram window generator.
+    :rtype: ``Generator[tuple[str], None, None]``
     """
     it = iter(seq)
     wd = deque((next(it, None) for _ in range(n)), maxlen=n)
 
     yield tuple(wd)
     for el in it:
         wd.append(el)
         yield tuple(wd)
 
 
 class BetterBM25DocumentStore:
     """
-    An in-memory document store intended to improve the default BM25 document
-    store shipped with Haystack.
+    An in-memory BM25 document store intended to improve the default
+    ``InMemoryDocumentStore`` shipped with Haystack.
     """
 
     default_sp_file: Final = os.path.join(
         os.path.dirname(os.path.abspath(__file__)), "default.model"
     )
+    """@private"""
 
     def __init__(
         self,
         *,
         k: float = 1.5,
         b: float = 0.75,
         delta: float = 1.0,
         sp_file: Optional[str] = None,
         n_grams: Union[int, tuple[int, int]] = 1,
         haystack_filter_logic: bool = True,
     ) -> None:
         """
-        Creates a new BetterBM25DocumentStore instance.
+        Creates a new ``BetterBM25DocumentStore`` instance.
 
-        An in-memory document store intended to improve the default
-        BM25 document store shipped with Haystack. The default store
-        recompute the index for the entire document store for every
-        in-coming query, which is significantly inefficient. This
-        store aims to improve the efficiency by pre-computing the
-        index for all documents in the store and only do incremental
-        updates when new documents are added or removed. Further, it
-        leverages a SentencePiece model to tokenize the input text
-        to allow more flexible and dynamic tokenization adapted to
-        domain-specific text.
-
-        :param k: the k1 parameter in BM25+ formula.
-        :type k: float, optional
-        :param b: the b parameter in BM25+ formula.
-        :type b: float, optional
-        :param delta: the delta parameter in BM25+ formula.
-        :type delta: float, optional
-        :param sp_file: the SentencePiece model file to use for
-            tokenization.
-        :type sp_file: Optional[str], optional
-        :param n_grams: the n-gram window size.
-        :type n_grams: Optional[Union[int, tuple[int, int]]], optional
-        :param haystack_filter_logic: Whether to use the Haystack
-            filter logic or the one implemented in this store,
-            which is more conservative.
-        :type haystack_filter_logic: bool, optional
+        :param k: k1 parameter in BM25+ formula.
+        :type k: ``Optional[float]``
+        :param b: b parameter in BM25+ formula.
+        :type b: ``Optional[float]``
+        :param delta: delta parameter in BM25+ formula.
+        :type delta: ``Optional[float]``
+        :param sp_file: ``SentencePiece`` tokenizer ``.model`` file to
+            use. A default from LLaMA-2-32K is used if not provided.
+        :type sp_file: ``Optional[str]``
+        :param n_grams: The n-gram window size. Can be a range of n-grams
+            to include in text representation. If a single integer is
+            provided, it will be treated as the maximum n-gram window size,
+            which is equivalent to ``(1, n_grams)``.
+        :type n_grams: ``Optional[Union[int, tuple[int, int]]]``
+        :param haystack_filter_logic: Whether to use the Haystack filter
+            logic or the one implemented in this store.
+        :type haystack_filter_logic: ``Optional[bool]``
         """
         self.k = k
+        """@private"""
+
         self.b = b
+        """@private"""
 
-        # Adjust the delta value so that we can bring the `(k1 + 1)`
-        # term out of the 'term frequency' term in BM25+ formula and
-        # delete it; this will not affect the ranking
         self.delta = delta / (self.k + 1.0)
+        """@private
+
+        Adjust the delta value so that we can bring the ``(k1 + 1)``
+        term out of the 'term frequency' term in BM25+ formula and
+        delete it; this will not affect the ranking.
+        """
 
         self._parse_sp_file(sp_file=sp_file)
         self._parse_n_grams(n_grams=n_grams)
 
         self._haystack_filter_logic = haystack_filter_logic
         self._filter_func = (
             document_matches_filter
@@ -165,19 +165,19 @@
         """
         Tokenize input text using SentencePiece model.
 
         The input text can either be a single string or a list of strings,
         such as a single user query or a group of raw document. The tokenized
         text will be augmented into set of n-grams based.
 
-        :param texts: the input text to tokenize.
-        :type texts: Union[str, list[str]]
+        :param texts: Input text to tokenize, queries or documents.
+        :type texts: ``Union[str, list[str]]``
 
-        :return: the tokenized text, with n-grams augmented.
-        :rtype: list[list[tuple[str]]]
+        :return: Tokenized and n-gram augmented texts.
+        :rtype: ``list[list[tuple[str]]]``
         """
 
         def _augment_to_n_grams(tokens: list[str]) -> list[tuple[str]]:
             it = (
                 _n_grams(tokens, n)
                 for n in range(self._n_grams_min, self._n_grams_max + 1)
             )
@@ -194,25 +194,27 @@
         self,
         query: str,
         documents: list[Document],
     ) -> list[tuple[Document, float]]:
         """
         Calculate the BM25+ score for all documents in this index.
 
-        :param query: the query to calculate the BM25+ score for.
-        :type query: str
-        :param documents: the pool of documents to calculate the BM25+ score for.
-        :type documents: list[Document]
+        :param query: Query to calculate the BM25+ score for.
+        :type query: ``str``
+        :param documents: Filtered pool of documents retrieve from.
+        :type documents: ``list[Document]``
 
-        :return: the BM25+ scores for all documents.
-        :rtype: list[tuple[Document, float]]
+        :return: Documents and corresponding BM25+ scores.
+        :rtype: ``list[tuple[Document, float]]``
         """
         cnt = lambda ng: self._freq_doc.get(ng, 0)
         idf = {
-            ng: math.log(1 + (len(self._index) - cnt(ng) + 0.5) / (cnt(ng) + 0.5))
+            ng: math.log(
+                1 + (self.count_documents() - cnt(ng) + 0.5) / (cnt(ng) + 0.5)
+            )
             for ng in self._tokenize(query)[0]
         }
 
         sim = []
         for doc in documents:
             _, freq, doc_len = self._index[doc.id]
             doc_len_scaled = doc_len / self._avg_doc_len
@@ -235,85 +237,93 @@
         *,
         filters: Optional[dict[str, Any]] = None,
         top_k: Optional[int] = None,
     ) -> list[tuple[Document, float]]:
         """
         Retrieve documents from the store using the given query.
 
-        :param query: the query to search for.
-        :type query: str
-        :param filters: the filters to apply to the document list.
-        :type filters: Optional[dict[str, Any]]
-        :param top_k: the number of documents to return.
-        :type top_k: int
+        :param query: Query to search for.
+        :type query: ``str``
+        :param filters: Filters to apply to the document list.
+        :type filters: ``Optional[dict[str, Any]]``
+        :param top_k: Number of documents to return.
+        :type top_k: ``int``
 
-        :return: the top-k documents and corresponding sim score.
-        :rtype: list[tuple[Document, float]]
+        :return: Top ``k`` documents and corresponding BM25+ scores.
+        :rtype: ``list[tuple[Document, float]]``
         """
         documents = self.filter_documents(filters)
         if not documents:
             return []
 
         sim = self._compute_bm25plus(query, documents)
         if top_k is None:
             return sorted(sim, key=lambda x: x[1], reverse=True)
         return heapq.nlargest(top_k, sim, key=lambda x: x[1])
 
     def count_documents(self) -> int:
         """
-        Returns how many documents are present in the document store.
+        Returns how many documents are present in this store.
 
-        :return: the number of documents in the store.
-        :rtype: int
+        :return: Number of documents in the store.
+        :rtype: ``int``
         """
-        return len(self._index)
+        return len(self._index.keys())
 
     def filter_documents(
         self, filters: Optional[dict[str, Any]] = None
     ) -> list[Document]:
         """
         Filter documents in the store using the given filters.
 
-        :param filters: the filters to apply to the document list.
-        :type filters: Optional[dict[str, Any]]
+        :param filters: Filters to apply to the document list.
+        :type filters: ``Optional[dict[str, Any]]``
 
-        :return: the list of documents that match the given filters.
-        :rtype: list[Document]
+        :return: List of documents that match the given filters.
+        :rtype: ``list[Document]``
         """
         if filters is None or not filters:
             return [doc for doc, _, _ in self._index.values()]
         return [
             doc
             for doc, _, _ in self._index.values()
             if self._filter_func(filters, doc)
         ]
 
     def write_documents(
         self,
         documents: list[Document],
-        policy: DuplicatePolicy = DuplicatePolicy.FAIL,
+        policy: DuplicatePolicy = DuplicatePolicy.NONE,
     ) -> int:
         """
         Writes (or overwrites) documents into the store.
 
-        :param documents: a list of documents.
-        :type documents: list[Document]
-        :param policy: documents with the same ID count as duplicates.
-            When duplicates are met, the store can:
-             - skip: keep the existing document and ignore the new one.
-             - overwrite: remove the old document and write the new one.
-             - fail: an error is raised
-        :type policy: DuplicatePolicy, optional
+        :param documents: List of documents to write.
+        :type documents: ``list[Document]``
+        :param policy: Documents with the same ``Document.id`` count as
+            duplicates. When duplicates are met, the store can:
+             - ``SKIP``: keep the existing document and ignore the new one.
+             - ``OVERWRITE``: remove the old document and write the new one.
+             - ``FAIL``: an error is raised (default behavior if not specified)
+        :type policy: ``Optional[DuplicatePolicy]``
 
+        :raises ValueError: Exception trigger on invalid duplicate policy.
         :raises DuplicateDocumentError: Exception trigger on duplicate
-            document if `policy=DuplicatePolicy.FAIL`
+            document if ``policy=DuplicatePolicy.FAIL``
 
         :return: Number of documents written.
-        :rtype: int
+        :rtype: ``int``
         """
+        if policy not in DuplicatePolicy:
+            msg = f"Invalid duplicate policy: {policy}."
+            raise ValueError(msg)
+
+        if policy == DuplicatePolicy.NONE:
+            policy = DuplicatePolicy.FAIL
+
         n_written = 0
         for doc in documents:
             if not isinstance(doc, Document):
                 msg = f"Expected document type, got '{doc}' of type '{type(doc)}'."
                 raise ValueError(msg)
 
             if doc.id in self._index.keys():
@@ -334,46 +344,43 @@
                 content = doc.dataframe.astype(str).to_csv(index=False)
 
             tokens = self._tokenize(content)[0]
 
             self._index[doc.id] = (doc, Counter(tokens), len(tokens))
             self._freq_doc.update(set(tokens))
             self._avg_doc_len = (
-                len(tokens) + self._avg_doc_len * len(self._index)
-            ) / (len(self._index) + 1)
+                len(tokens) + self._avg_doc_len * self.count_documents()
+            ) / (self.count_documents() + 1)
 
             logger.debug(f"Document '{doc.id}' written to store.")
             n_written += 1
 
         return n_written
 
     def delete_documents(self, document_ids: list[str]) -> int:
         """
-        Deletes all documents with a matching document_ids.
-
-        Fails with `MissingDocumentError` if no document with
-        this id is present in the store.
+        Deletes all documents with a matching ID.
 
-        :param object_ids: the object_ids to delete
-        :type object_ids: list[str]
+        :param document_ids: List of ``object_id`` to delete
+        :type document_ids: ``list[str]``
 
-        :raises MissingDocumentError: trigger on missing document.
+        :raises MissingDocumentError: Triggered on document not found.
 
         :return: Number of documents deleted.
-        :rtype: int
+        :rtype: ``int``
         """
         n_removal = 0
         for doc_id in document_ids:
             try:
                 _, freq, doc_len = self._index.pop(doc_id)
                 self._freq_doc.subtract(Counter(freq.keys()))
                 try:
                     self._avg_doc_len = (
-                        self._avg_doc_len * (len(self._index) + 1) - doc_len
-                    ) / len(self._index)
+                        self._avg_doc_len * (self.count_documents() + 1) - doc_len
+                    ) / self.count_documents()
                 except ZeroDivisionError:
                     self._avg_doc_len = 0
 
                 logger.debug(f"Document '{doc_id}' deleted from store.")
                 n_removal += 1
             except KeyError as exc:
                 msg = f"Document with ID '{doc_id}' not found, cannot delete it."
```

### Comparing `bbm25_haystack-0.2.0/src/bbm25_haystack/default.model` & `bbm25_haystack-0.2.1/src/bbm25_haystack/default.model`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/src/bbm25_haystack/filters.py` & `bbm25_haystack-0.2.1/src/bbm25_haystack/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,33 @@
 from haystack.errors import FilterError
 
 
 def apply_filters_to_document(
     filters: Optional[dict[str, Any]], document: Document
 ) -> bool:
     """
-    Apply filters to a document.
+    Apply filters to a document. Differences with the official
+    Haystack implementation:
+
+    - Comparison with ``None``, i.e., missing values, involved will
+        always return ``False``, no matter missing the document
+        attribute value or missing the filter value.
+    - Comparison with ``pandas.DataFrame`` is always prohibited to
+        reduce surprises.
+    - No implicit ``datetime`` conversion from string values.
+    - ``in`` and ``not in`` allows any ``Iterable`` as filter value,
+        without the ``list`` constraint.
 
     :param filters: The filters to apply to the document.
-    :type filters: dict[str, Any]
+    :type filters: ``dict[str, Any]``
     :param document: The document to apply the filters to.
-    :type document: Document
+    :type document: ``Document``
 
-    :return: True if the document passes the filters.
-    :rtype: bool
+    :return: ``True`` if the document passes the filters.
+    :rtype: ``bool``
     """
     if filters is None or not filters:
         return True
     return _run_comparison_condition(filters, document)
 
 
 def _get_document_field(document: Document, field: str) -> Optional[Any]:
```

### Comparing `bbm25_haystack-0.2.0/tests/test_document_store.py` & `bbm25_haystack-0.2.1/tests/test_document_store.py`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/tests/test_retriever.py` & `bbm25_haystack-0.2.1/tests/test_retriever.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
             result["documents"][0].content == "PHP is a popular programming language"
         )
 
     def test_invalid_run_wrong_store_type(self):
         store_class = document_store_class("SomeOtherDocumentStore")
         with pytest.raises(
             TypeError,
-            match="document_store must be an instance of BetterBM25DocumentStore",
+            match="'document_store' must be of type 'BetterBM25DocumentStore'",
         ):
             BetterBM25Retriever(store_class())
 
     @pytest.mark.integration
     @pytest.mark.parametrize(
         "query, query_result",
         [
```

### Comparing `bbm25_haystack-0.2.0/.gitignore` & `bbm25_haystack-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/LICENSE` & `bbm25_haystack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/README.md` & `bbm25_haystack-0.2.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -20,56 +20,70 @@
 $ git clone https://github.com/Guest400123064/bbm25-haystack.git
 $ cd bbm25-haystack
 $ pip install -e .
 ```
 
 ## Usage
 
-The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, one path to a trained SentencePiece tokenizer `.model` file, and a filtering logic flag ([see below](#filtering-logic)). All parameters are optional. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
+### Quick Start
+
+Below is an example of how you can build a minimal search engine with the `bbm25_haystack` components on their own. They are also compatible with [Haystack pipelines](https://docs.haystack.deepset.ai/docs/creating-pipelines).
 
 ```python
 from haystack import Document
 from bbm25_haystack import BetterBM25DocumentStore, BetterBM25Retriever
 
 
 document_store = BetterBM25DocumentStore()
 document_store.write_documents([
    Document(content="There are over 7,000 languages spoken around the world today."),
    Document(content="Elephants have been observed to behave in a way that indicates a high level of self-awareness, such as recognizing themselves in mirrors."),
-   Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bioluminescent waves.")
+   Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bio-luminescent waves.")
 ])
 
 retriever = BetterBM25Retriever(document_store)
 retriever.run(query="How many languages are spoken around the world today?")
 ```
 
+### API References
+
+You can find the full API references [here](https://guest400123064.github.io/bbm25-haystack/). In a hurry? Below are some most important document store parameters you might want explore:
+
+- `k, b, delta` - the [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25).
+- `sp_file` - a path to a trained SentencePiece tokenizer `.model` file. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
+- `n_grams` - default to 1, which means text (both query and document) are tokenized into unigrams. If set to 2, the tokenizer also augment the list of uni-grams with bi-grams, and so on. If specified as tuple, e.g., (2, 3), the tokenizer only produce bi-grams and tri-grams, without any uni-gram.
+- `haystack_filter_logic` - see [below](#filtering-logic).
+
+The retriever parameters are largely the same as [`InMemoryBM25Retriever`](https://docs.haystack.deepset.ai/docs/inmemorybm25retriever).
+
 ## Filtering Logic
 
-The current document store uses `document_matches_filter` shipped with Haystack to perform filtering by default, which is the same as `InMemoryDocumentStore` except that it is DOES NOT support legacy operator names.
+The current document store uses [`document_matches_filter`](https://github.com/deepset-ai/haystack/blob/main/haystack/utils/filters.py) shipped with Haystack to perform filtering by default, which is the same as [`InMemoryDocumentStore`](https://docs.haystack.deepset.ai/docs/inmemorydocumentstore).
 
-However, there is also an alternative filtering logic shipped with this implementation that is more conservative (and unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False` Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
+However, there is also an alternative filtering logic shipped with this implementation (unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False`. Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
 
-- Comparison with `None`, i.e., missing values, involved will always return `False`, no matter the document attribute value or filter value.
-- Comparison with `DataFrame` is always prohibited to reduce surprises.
+- Comparison with `None`, i.e., missing values, involved will always return `False`, no matter missing the document attribute value or missing the filter value.
+- Comparison with `pandas.DataFrame` is always prohibited to reduce surprises.
 - No implicit `datetime` conversion from string values.
+- `in` and `not in` allows any `Iterable` as filter value, without the `list` constraint.
 
-These differences lead to a few caveats. Firstly, some test cases are overridden to take into account the different expectations. However, this means that passed, non-overridden tests may not be faithful, i.e., the filters behave in the same way as the old implementation while different behaviors are expected. Further, the negation logic needs to be considered again because `False` can now issue from both input check and the actual comparisons. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
+In this case, the negation logic needs to be considered again because `False` can now issue from both input nullity check and the actual comparisons. For instance, `in` and `not in` both yield non-matching upon missing values. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
 
 ## Search Quality Evaluation
 
 This repo has [a simple script](./scripts/benchmark_beir.py) to help evaluate the search quality over [BEIR](https://github.com/beir-cellar/beir/tree/main) benchmark. You need to clone the repository (you can also manually download the script and place it under a folder named `scripts`) and you have to install additional dependencies to run the script.
 
 ```bash
 $ pip install beir
 ```
 
 To run the script, you may want to specify the dataset name and BM25 hyperparameters. For example:
 
 ```bash
-$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --output eval.csv
+$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --n-grams 2 --output eval.csv
 ```
 
 It automatically downloads the benchmarking dataset to `benchmarks/beir`, where `benchmarks` is at the same level as `scripts`. You may also check the help page for more information.
 
 ```bash
 $ python scripts/benchmark_beir.py --help
 ```
```

### Comparing `bbm25_haystack-0.2.0/pyproject.toml` & `bbm25_haystack-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bbm25_haystack-0.2.0/PKG-INFO` & `bbm25_haystack-0.2.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bbm25-haystack
-Version: 0.2.0
+Version: 0.2.1
 Summary: Haystack 2.x In-memory Document Store with Enhanced Efficiency
 Project-URL: Documentation, https://github.com/Guest400123064/bbm25-haystack#readme
 Project-URL: Issues, https://github.com/Guest400123064/bbm25-haystack/issues
 Project-URL: Source, https://github.com/Guest400123064/bbm25-haystack
 Author-email: Yuxuan Wang <wangy49@seas.upenn.edu>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -44,56 +44,70 @@
 $ git clone https://github.com/Guest400123064/bbm25-haystack.git
 $ cd bbm25-haystack
 $ pip install -e .
 ```
 
 ## Usage
 
-The initializer takes [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25), namely `k1`, `b`, and `delta`, one path to a trained SentencePiece tokenizer `.model` file, and a filtering logic flag ([see below](#filtering-logic)). All parameters are optional. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
+### Quick Start
+
+Below is an example of how you can build a minimal search engine with the `bbm25_haystack` components on their own. They are also compatible with [Haystack pipelines](https://docs.haystack.deepset.ai/docs/creating-pipelines).
 
 ```python
 from haystack import Document
 from bbm25_haystack import BetterBM25DocumentStore, BetterBM25Retriever
 
 
 document_store = BetterBM25DocumentStore()
 document_store.write_documents([
    Document(content="There are over 7,000 languages spoken around the world today."),
    Document(content="Elephants have been observed to behave in a way that indicates a high level of self-awareness, such as recognizing themselves in mirrors."),
-   Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bioluminescent waves.")
+   Document(content="In certain parts of the world, like the Maldives, Puerto Rico, and San Diego, you can witness the phenomenon of bio-luminescent waves.")
 ])
 
 retriever = BetterBM25Retriever(document_store)
 retriever.run(query="How many languages are spoken around the world today?")
 ```
 
+### API References
+
+You can find the full API references [here](https://guest400123064.github.io/bbm25-haystack/). In a hurry? Below are some most important document store parameters you might want explore:
+
+- `k, b, delta` - the [three BM25+ hyperparameters](https://en.wikipedia.org/wiki/Okapi_BM25).
+- `sp_file` - a path to a trained SentencePiece tokenizer `.model` file. The default tokenizer is directly copied from [LLaMA-2-7B-32K tokenizer](https://huggingface.co/togethercomputer/LLaMA-2-7B-32K/blob/main/tokenizer.model) with a vocab size of 32,000.
+- `n_grams` - default to 1, which means text (both query and document) are tokenized into unigrams. If set to 2, the tokenizer also augment the list of uni-grams with bi-grams, and so on. If specified as tuple, e.g., (2, 3), the tokenizer only produce bi-grams and tri-grams, without any uni-gram.
+- `haystack_filter_logic` - see [below](#filtering-logic).
+
+The retriever parameters are largely the same as [`InMemoryBM25Retriever`](https://docs.haystack.deepset.ai/docs/inmemorybm25retriever).
+
 ## Filtering Logic
 
-The current document store uses `document_matches_filter` shipped with Haystack to perform filtering by default, which is the same as `InMemoryDocumentStore` except that it is DOES NOT support legacy operator names.
+The current document store uses [`document_matches_filter`](https://github.com/deepset-ai/haystack/blob/main/haystack/utils/filters.py) shipped with Haystack to perform filtering by default, which is the same as [`InMemoryDocumentStore`](https://docs.haystack.deepset.ai/docs/inmemorydocumentstore).
 
-However, there is also an alternative filtering logic shipped with this implementation that is more conservative (and unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False` Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
+However, there is also an alternative filtering logic shipped with this implementation (unstable at this point). To use this alternative logic, initialize the document store with `haystack_filter_logic=False`. Please find comments and implementation details in [`filters.py`](./src/bbm25_haystack/filters.py). TL;DR:
 
-- Comparison with `None`, i.e., missing values, involved will always return `False`, no matter the document attribute value or filter value.
-- Comparison with `DataFrame` is always prohibited to reduce surprises.
+- Comparison with `None`, i.e., missing values, involved will always return `False`, no matter missing the document attribute value or missing the filter value.
+- Comparison with `pandas.DataFrame` is always prohibited to reduce surprises.
 - No implicit `datetime` conversion from string values.
+- `in` and `not in` allows any `Iterable` as filter value, without the `list` constraint.
 
-These differences lead to a few caveats. Firstly, some test cases are overridden to take into account the different expectations. However, this means that passed, non-overridden tests may not be faithful, i.e., the filters behave in the same way as the old implementation while different behaviors are expected. Further, the negation logic needs to be considered again because `False` can now issue from both input check and the actual comparisons. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
+In this case, the negation logic needs to be considered again because `False` can now issue from both input nullity check and the actual comparisons. For instance, `in` and `not in` both yield non-matching upon missing values. But I think having input processing and comparisons separated makes the filtering behavior more transparent.
 
 ## Search Quality Evaluation
 
 This repo has [a simple script](./scripts/benchmark_beir.py) to help evaluate the search quality over [BEIR](https://github.com/beir-cellar/beir/tree/main) benchmark. You need to clone the repository (you can also manually download the script and place it under a folder named `scripts`) and you have to install additional dependencies to run the script.
 
 ```bash
 $ pip install beir
 ```
 
 To run the script, you may want to specify the dataset name and BM25 hyperparameters. For example:
 
 ```bash
-$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --output eval.csv
+$ python scripts/benchmark_beir.py --datasets scifact arguana --bm25-k1 1.2 --n-grams 2 --output eval.csv
 ```
 
 It automatically downloads the benchmarking dataset to `benchmarks/beir`, where `benchmarks` is at the same level as `scripts`. You may also check the help page for more information.
 
 ```bash
 $ python scripts/benchmark_beir.py --help
 ```
```

