Keywords: Golang, go, document database, NoSQL, JSON

<img src="http://golang.org/doc/gopher/frontpage.png" alt="Golang logo" align="right"/>

### tiedot - Your NoSQL database powered by Golang

tiedot is a document database that uses __JSON__ for documents and queries; it can be __embedded__ into your program, or run a stand-alone server using __HTTP__ for an API.

### Feature Highlights

- Designed for both embedded usage and standalone service.
- Fault-tolerant data structures that put safety of your data *first*.
- Very scalable on SMP computers.
- Use JSON syntax to build powerful queries.
- Support both \*nix and Windows operating systems.

### High Performance!

tiedot scales very well on SMP computers. Here are results collected from tiedot built-in benchmarks:

(Operations per second)
<table>
<tr>
  <th>Processor</th>
  <th>Insert</th>
  <th>Read</th>
  <th>Query</th>
  <th>Update</th>
  <th>Delete</th>
  <th>Mix*</th>
  <th>Machine Type</th>
</tr>
<tr>
  <td>Mobile Intel Core i7 2.8GHZ</td>
  <td>345,000</td>
  <td>680,000</td>
  <td>155,000</td>
  <td>200,000</td>
  <td>490,000</td>
  <td>435,000</td>
  <td>2013 model MacBook</td>
</tr>
<tr>
  <td>Mobile Intel Core i7 1.8GHZ</td>
  <td>147,000</td>
  <td>290,000</td>
  <td>65,000</td>
  <td>75,000</td>
  <td>190,000</td>
  <td>155,000</td>
  <td>2011 model laptop</td>
</tr>
<tr>
  <td>Amazon EC2 c1.medium</td>
  <td>54,000</td>
  <td>117,000</td>
  <td>29,000</td>
  <td>31,000</td>
  <td>85,000</td>
  <td>65,000</td>
  <td>A medium range instance</td>
</tr>
</table>

Mix\* runs simultaneous insert/read/update/delete/query operations. See [Performance tuning and benchmarks] for more details

> Did you know? The largest known tiedot deployment powers a personal offline Wikipedia indexing project, it has 5.9 million documents and over 73GB of data.

> Your contribution means a lot to tiedot! Please read [ways to contribute][].

### References

- [Quick Start Guide: tiedot in 10 minutes]
- [API reference (V3)]
- [Embedded usage]
- [Data structures]
- [Query processor and index]
- [Concurrency and networking]
- [Performance tuning and benchmarks]
- [Limitations]

### Version History

See [Version History] for detailed change logs, known issues, etc.

<table>
<tr>
  <th>Version (and branch name)</th>
  <th>Release Date</th>
  <th>Highlights</th>
</tr>
<tr>
  <td>Alpha</td>
  <td>2013-06-28</td>
  <td>First release</td>
</tr>
<tr>
  <td>Beta</td>
  <td>2013-07-12</td>
  <td>Platform support and data durability improvements.</td>
</tr>
<tr>
  <td>1.0</td>
  <td>2013-09-21</td>
  <td>Query performance/syntax, and documentation improvements.</td>
</tr>
<tr>
  <td>1.1</td>
  <td>2013-10-06</td>
  <td>Memory consumption improvements; persistent document ID system.</td>
</tr>
</table>

### Contact and License

Future development plans are tracked in [Issues] section.

For feedback and questions, please contact [Howard] - I would love to hear from you! Please also check out my [Twitter] and [blog].

Please check out [Contributors and License].

### Project Background

__Is tiedot "yet another NoSQL database"?__

There are probably as many NoSQL database as there are Linux distributions.

tiedot is not as powerful (yet) - and does not intend to compete with mainstream NoSQL database engines such as CouchDB or Cassandra. However, tiedot performs reasonably well given its small size (around 3k LOC); and due to its simplicity, its performance may come close or even exceed those large brand NoSQL solutions (under certain workloads).

__What is the motive behind this project?__

Golang (Go) is a fascinating language - very easy to use, scalable and reasonably stable. I am very passionate about document database technologies (check out my other GitHub projects!) and enjoy seeing my code scaling well on SMP machines. This is my Golang exercise.

__Why the name "tiedot"?__

"tiedot" is a Finnish word standing for "data". I enjoy learning (natural and computer) languages, also enjoy listening to music in many languages. "Tiedot" sounds cute, doesn't it?

[Quick Start Guide: tiedot in 10 minutes]: https://github.com/HouzuoGuo/tiedot/wiki/Tutorial
[API reference (V3)]: https://github.com/HouzuoGuo/tiedot/wiki/API-V3-Reference
[Version History]: https://github.com/HouzuoGuo/tiedot/wiki/Version-History
[Embedded usage]: https://github.com/HouzuoGuo/tiedot/wiki/Embedded-Usage
[Data structures]: https://github.com/HouzuoGuo/tiedot/wiki/Data-structures
[Query processor and index]: https://github.com/HouzuoGuo/tiedot/wiki/Query-processor-and-index
[Concurrency and networking]: https://github.com/HouzuoGuo/tiedot/wiki/Concurrency-and-networking
[Performance tuning and benchmarks]: https://github.com/HouzuoGuo/tiedot/wiki/Performance-tuning-and-benchmarks
[Limitations]: https://github.com/HouzuoGuo/tiedot/wiki/Limitations
[Howard]: mailto:guohouzuo@gmail.com
[Twitter]: https://twitter.com/hzguo
[blog]: http://allstarnix.blogspot.com.au
[Issues]: https://github.com/HouzuoGuo/tiedot/issues
[Contributors and License]: https://github.com/HouzuoGuo/tiedot/wiki/Contributors-and-License
[ways to contribute]: https://github.com/HouzuoGuo/tiedot/wiki/ways-to-contribute