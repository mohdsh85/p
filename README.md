Data analysis with Python

In this course an overview is given of different phases of the data analysis pipeline using Python and its data analysis ecosystem. What is typically done in data analysis? We assume that data is already available, so we only need to download it. After downloading the data it needs to be cleaned to enable further analysis. In the cleaning phase the data is converted to some uniform and consistent format. After which the data can, for instance, be

    combined or divided into smaller chunks
    grouped or sorted,
    condensed into small number of summary statistics
    numerical or string operations can be performed on the data

The point is to manipulate the data into a form that enables discovery of relationships and regularities among the elements of data. Visualization of data often helps to get a better understanding of the data. Another useful tool for data analysis is machine learning, where a mathematical or statistical model is fitted to the data. These models can then be used to make predictions of new data, or can be used to explain or describe the current data.

Python is a popular, easy to learn programming language. It is commonly used in the field of data analysis, because there are very efficient libraries available to process large amounts of data. This so called data analysis stack includes libraries such of NumPy, Pandas, Matplotlib and SciPy.

No previous knowledge of Python is needed as will start with a quick introduction to Python. It is however assumed that you have good programming skills in some language. 


<div class="section" id="software-libraries-used">
<h2>Software libraries used<a class="headerlink" href="#software-libraries-used" title="Permalink to this headline">¶</a></h2>
<div class="wy-table-responsive"><table class="docutils" border="1">
<colgroup>
<col width="20%">
<col width="80%">
</colgroup>
<thead valign="bottom">
<tr class="row-odd"><th class="head" rowspan="2">Library</th>
<th class="head" rowspan="2">Documentation</th>
</tr>
<tr class="row-even"></tr>
</thead>
<tbody valign="top">
<tr class="row-odd"><td>numpy</td>
<td><a class="reference external" href="https://docs.scipy.org/doc/numpy/">doc</a></td>
</tr>
<tr class="row-even"><td>pandas</td>
<td><a class="reference external" href="http://pandas.pydata.org/pandas-docs/stable/">doc</a></td>
</tr>
<tr class="row-odd"><td>matplotlib</td>
<td><a class="reference external" href="https://matplotlib.org/api/api_overview.html">doc</a></td>
</tr>
<tr class="row-even"><td>scikit-learn</td>
<td><a class="reference external" href="https://scikit-learn.org/stable/">doc</a></td>
</tr>
<tr class="row-odd"><td>scipy</td>
<td><a class="reference external" href="https://docs.scipy.org/doc/scipy/reference/">doc</a></td>
</tr>
</tbody>
</table></div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Contents:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="instructions.html">Initializing course environment</a><ul>
<li class="toctree-l2"><a class="reference internal" href="instructions.html#1-Install-Python-and-the-needed-external-packages">1 Install Python and the needed external packages</a></li>
<li class="toctree-l2"><a class="reference internal" href="instructions.html#2-Log-in-to-the-course">2 Log in to the course</a></li>
<li class="toctree-l2"><a class="reference internal" href="instructions.html#3-Install-TMC-client">3 Install TMC client</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="tools.html">Running Python code</a><ul>
<li class="toctree-l2"><a class="reference internal" href="tools.html#ipython">IPython</a></li>
<li class="toctree-l2"><a class="reference internal" href="tools.html#jupyter-notebook">Jupyter notebook</a></li>
<li class="toctree-l2"><a class="reference internal" href="tools.html#executing-a-file-containing-python-code">Executing a file containing Python code</a></li>
<li class="toctree-l2"><a class="reference internal" href="tools.html#correct-software-versions">Correct software versions</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="faq.html">Frequently asked questions</a><ul>
<li class="toctree-l2"><a class="reference internal" href="faq.html#when-logging-to-tmc-first-time-whats-the-server-address-it-asks">When logging to tmc first time, whats the server address it asks?</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#tmc-login-crashes-with-mention-of-tmc-cli-log">TMC login crashes (with mention of tmc-cli.log)</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#tmc-test-fails-but-all-other-commands-including-submit-work">TMC test fails but all other commands (including submit) work</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#stuff-generally-doesn-t-seem-to-work-in-the-conda-prompt-on-windows">Stuff generally doesn’t seem to work in the conda prompt on Windows</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#tmc-not-found">tmc not found</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#tmc-test-says-test-results-0-0-tests-passed"><cite>tmc test</cite> says: “Test results: 0/0 tests passed”</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#what-version-of-python-should-i-use-what-is-the-name-of-the-executable">What version of Python should I use? What is the name of the executable?</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#how-to-load-a-file-that-resides-in-the-src-folder">How to load a file that resides in the src folder?</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#tests-complain-about-missing-attribute-assert-called-assert-called-once">Tests complain about missing attribute assert_called, assert_called_once, …</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#modulenotfounderror-no-module-named-somelibrary">ModuleNotFoundError: No module named ‘somelibrary’</a></li>
<li class="toctree-l2"><a class="reference internal" href="faq.html#i-cannot-understand-the-error-message-from-a-failed-test-case">I cannot understand the error message from a failed test case</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week 1:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="basics.html">Python</a><ul>
<li class="toctree-l2"><a class="reference internal" href="basics.html#Basic-concepts">Basic concepts</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics.html#String-handling">String handling</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics.html#Modules">Modules</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics.html#Summary">Summary</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week 2:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="basics2.html">Python (continues)</a><ul>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#Regular-expressions">Regular expressions</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#Basic-file-processing">Basic file processing</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#sys-module">sys module</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#Objects-and-classes">Objects and classes</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#Exceptions">Exceptions</a></li>
<li class="toctree-l2"><a class="reference internal" href="basics2.html#Sequences,-iterables,-generators:-revisited">Sequences, iterables, generators: revisited</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="numpy.html">NumPy</a><ul>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Creation-of-arrays">Creation of arrays</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Array-types-and-attributes">Array types and attributes</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Indexing,-slicing-and-reshaping">Indexing, slicing and reshaping</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Array-concatenation,-splitting-and-stacking">Array concatenation, splitting and stacking</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Fast-computation-using-universal-functions">Fast computation using universal functions</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Aggregations:-max,-min,-sum,-mean,-standard-deviation...">Aggregations: max, min, sum, mean, standard deviation…</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Broadcasting">Broadcasting</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy.html#Summary-(week-2)">Summary (week 2)</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week 3:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="numpy2.html">NumPy (continues)</a><ul>
<li class="toctree-l2"><a class="reference internal" href="numpy2.html#Comparisons-and-masking">Comparisons and masking</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy2.html#Fancy-indexing">Fancy indexing</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy2.html#Sorting-arrays">Sorting arrays</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy2.html#Matrix-operations">Matrix operations</a></li>
<li class="toctree-l2"><a class="reference internal" href="numpy2.html#Solving-system-of-linear-equations">Solving system of linear equations</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="matplotlib.html">Matplotlib</a><ul>
<li class="toctree-l2"><a class="reference internal" href="matplotlib.html#Simple-figure">Simple figure</a></li>
<li class="toctree-l2"><a class="reference internal" href="matplotlib.html#Subfigures">Subfigures</a></li>
<li class="toctree-l2"><a class="reference internal" href="matplotlib.html#Other-data-visualization-libraries-for-Python">Other data visualization libraries for Python</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="image_processing.html">Image processing</a><ul>
<li class="toctree-l2"><a class="reference internal" href="image_processing.html#Finding-clusters-in-an-image">Finding clusters in an image</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="pandas1.html">Pandas</a><ul>
<li class="toctree-l2"><a class="reference internal" href="pandas1.html#Creation-and-indexing-of-series">Creation and indexing of series</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas1.html#Summary-(week-3)">Summary (week 3)</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week 4:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="pandas2.html">Pandas (continues)</a><ul>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Creation-of-dataframes">Creation of dataframes</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Accessing-columns-and-rows-of-a-dataframe">Accessing columns and rows of a dataframe</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Alternative-indexing-and-data-selection">Alternative indexing and data selection</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Summary-statistics">Summary statistics</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Missing-data">Missing data</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Converting-columns-from-one-type-to-another">Converting columns from one type to another</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#String-processing">String processing</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Additional-information">Additional information</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas2.html#Summary-(week-4)">Summary (week 4)</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week 5:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="pandas3.html">Pandas (continues)</a><ul>
<li class="toctree-l2"><a class="reference internal" href="pandas3.html#Catenating-datasets">Catenating datasets</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas3.html#Merging-dataframes">Merging dataframes</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas3.html#Aggregates-and-groupings">Aggregates and groupings</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas3.html#Time-series">Time series</a></li>
<li class="toctree-l2"><a class="reference internal" href="pandas3.html#Additional-information">Additional information</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="linear_regression.html">Machine learning: linear regression</a><ul>
<li class="toctree-l2"><a class="reference internal" href="linear_regression.html#Linear-regression">Linear regression</a></li>
<li class="toctree-l2"><a class="reference internal" href="linear_regression.html#Additional-information">Additional information</a></li>
<li class="toctree-l2"><a class="reference internal" href="linear_regression.html#Summary-(week-5)">Summary (week 5)</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week6:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="bayes.html">ML: Naive Bayes classification</a><ul>
<li class="toctree-l2"><a class="reference internal" href="bayes.html#Another-example">Another example</a></li>
<li class="toctree-l2"><a class="reference internal" href="bayes.html#Text-classification">Text classification</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="clustering.html">ML: Clustering</a><ul>
<li class="toctree-l2"><a class="reference internal" href="clustering.html#Simple-example">Simple example</a></li>
<li class="toctree-l2"><a class="reference internal" href="clustering.html#More-complicated-example">More complicated example</a></li>
<li class="toctree-l2"><a class="reference internal" href="clustering.html#Clustering-digits">Clustering digits</a></li>
<li class="toctree-l2"><a class="reference internal" href="clustering.html#Hierarchical-clustering">Hierarchical clustering</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="pca.html">ML: Principal component analysis</a><ul>
<li class="toctree-l2"><a class="reference internal" href="pca.html#Principal-component-analysis">Principal component analysis</a></li>
<li class="toctree-l2"><a class="reference internal" href="pca.html#Summary-(week-6)">Summary (week 6)</a></li>
</ul>
</li>
</ul>
</div>
<div class="toctree-wrapper compound">
<p class="caption"><span class="caption-text">Week7:</span></p>
<ul>
<li class="toctree-l1"><a class="reference internal" href="project.html">Project work</a><ul>
<li class="toctree-l2"><a class="reference internal" href="project.html#sequence-analysis">Sequence analysis</a></li>
<li class="toctree-l2"><a class="reference internal" href="project.html#regression-analysis">Regression analysis</a></li>
</ul>
</li>
<li class="toctree-l1"><a class="reference internal" href="project.html#running-tests-when-peer-reviewing-students-notebooks">Running tests when peer-reviewing students notebooks</a><ul>
<li class="toctree-l2"><a class="reference internal" href="project.html#id1">Regression analysis</a></li>
<li class="toctree-l2"><a class="reference internal" href="project.html#id2">Sequence analysis</a></li>
</ul>
</li>
</ul>
</div>
</div>
