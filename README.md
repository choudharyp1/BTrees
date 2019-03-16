# BTrees
<h1>Implementation of B-trees</h1>

<p>A implementation of the insert, search and print functions of B-Trees. I have implemented this data structure as a part of my IB Extended Essay, where based on my implementation of the B-Trees, I calculate its effiecieny using <b>Big-O notation</b> to compare with the efficiency of "Extendible Hash Tables" to determine which data structure is more superior.</p>

<h2><b>Research Question:</b> </h2>
<h3>
To what Extent does the structure of a B-Tree make it a better choice than Extendible Hash Tables for creating database indexes?<h3>

<h2>Investigation:</h2>

<p>
Both B-Trees and Extendible Hash Tables have their own merits. Comparing both database structures in the basis of their basic insert and delete functions as well as, search queries. Search queries are also dependent on the type: Exact vs Range Queries.
</p>

<p>
We have to understand what is being measured when calculating the efficiency of the data structure algorithms. For this research, we count the number of disk access that each data structure will have to perform when executing a exact or range query.
</p>

<p>
Finally, we compare the potential performance of both database indexes if used to index the Oxford English Corpus, a gigantic database storing more than 2 Billion words and phrases.
</p>


<h3>Results and Conclusion:</h3>

<p>In queries and functions that require searching for a single item from the data structure, the key of the item being searched for is known. In this case, Extendible Hash Tables searches the item in constant time O(1). The query requires calculating the bucket ID using the hash functions and a single disk access to retrieve the bucket from secondary to primary memory.</p>
<p>
For range queries, where more than 1 item is being retrieved from the data structures, range queries prove to be a better choice because of the arrangement of the data stored. B-trees store data in a standard order. If storing numbers, it uses ascending or descending order. If storing letters, they are stored lexicographically. This allows them to estimate the location of the desired data and retrieve it in fewer disk accesses as compared to hash tables that would have to search every table to find the desired data because this structure orders data into buckets using hash functions instead.

<p>In conclusion, while both database indexes are incredible powerful, my investigation suggests that B-trees overall are a better choice than Extendible hash tables because this the tree can perform both types of queries very efficiently while the hash tables are highly efficient in exact queries however become very inefficient when running range queries.</p>
</p>



<h4>To read Extended essay with more details on my investigation on these two amazing data structures, click here:</h4>
<a href="https://github.com/choudharyp1/BTrees/blob/master/Pratik%20Choudhary%20Extended%20Essay%20Computer%20Science%20Final.pdf">IB Computer Science Extended Essay</a>
