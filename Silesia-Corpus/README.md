# The Silesia Corpus

The intention of the Silesia corpus is to provide a data set of files that covers the typical data types used nowadays. The sizes of the files are between 6 MB and 51 MB.

The chosen files are of different types and come from several sources. In our opinion, nowadays the two fastest growing types of data are multimedia and databases. The former are typically compressed with lossy methods so we do not include them in the corpus. The database files, osdb, sao, nci, come from three different fields. The first one is a sample database from an open source project that is intended to be used as a standard, free database benchmark. The second one, sao, is one of the astronomical star catalogues. This is a binary database composed of records of complex structure. The last one, nci, is a part of the chemical database of structures.

The sizes of computer programs are also growing rapidly. The standard corpora include only single, small routines, both in source and object code. Today it is almost impractical to compress every single source code file separately. The projects are composed of hundreds or thousands files, so it is a common habit to compress it all together. We often can achieve a better compression ratio if we compress a concatenated file of similar contents than the small separate ones. This trend is reflected in including a samba file. Besides the source codes, there is also a need to store the executables. We decided to include two files: ooffice and mozilla. The first one is a single medium-sized executable for the Windows system. The second is a concatenation of the whole application for Tru64 Unix system composed of executables, archives, texts, HTML files, and other.

There are also types of images that cannot be compressed loosely—the medical images. The sizes of such files are also huge and we include two examples of them in the corpus. The first file, x-ray, is an X-ray picture of a child's hand. The second file, mr, is a magnetic resonance, three dimensional image of a head.

The standard corpora contain text files. Moreover, these files are typically the largest files of them, but in our opinion there is a need to test the compression efficiency also on the larger ones stored in different file types. We propose three such files. The first, dickens, is a collection of some works by Charles Dickens that can be found in the Project Gutenberg. This is a plain text file. The second one, reymont, is a book Chłopi by Władysław Reymont stored in a PDF file. The PDF files can be internally-compressed but the quality of this build-in compression is rather poor, and much better results can be obtained when we compress an uncompressed PDF file. Because of this we enclose the uncompressed version. The last text file, webster, is an electronic version of The 1913 Webster Unabridged Dictionary taken from the Project Gutenberg. The file is stored in the HTML format. The last file of the new corpus, xml, is a concatenation of 21 XML files. The XML standard is designed to be a universal file format for storing documents, so we decided to enclose it.

There are 12 files in the Silesia Corpus:

| Filename | Description                                                   | Type        | Source                                            | Raw size [B] |
|----------|---------------------------------------------------------------|-------------|---------------------------------------------------|--------------|
| dickens  | Collected works of Charles Dickens                            | English text| Project Gutenberg                                 | 10,192,446   |
| mozilla  | Tarred executables of Mozilla 1.0 (Tru64 UNIX edition)        | exe         | Mozilla Project                                   | 51,220,480   |
| mr       | Medical magnetic resonance image                              | picture     | Hospital image                                    | 9,970,564    |
| nci      | Chemical database of structures                               | database    | CACTVS Chemical Information Services at LMC/NCI   | 33,553,445   |
| ooffice  | A dll from Open Office.org 1.01                               | exe         | Open Office                                       | 6,152,192    |
| osdb     | Sample database in MySQL format from Open Source Database Benchmark | database | Open Source Database Benchmark Project            | 10,085,684   |
| reymont  | Text of the book Chłopi by Władysław Reymont                  | Polish pdf  | Virtual Library of Polish Literature              | 6,627,202    |
| samba    | Tarred source code of Samba 2-2.3                             | src         | Samba Project                                     | 21,606,400   |
| sao      | The SAO star catalog                                          | bin data    | Astronomical Catalogs and Catalog Formats         | 7,251,944    |
| webster  | The 1913 Webster Unabridged Dictionary                        | html        | Project Gutenberg                                 | 41,458,703   |
| xml      | Collected XML files                                           | html        | XMLPPM: XML-Conscious PPM Compression             | 5,345,280    |
| x-ray    | X-ray medical picture                                         |             | Hospital image                                    | 8,474,240    |
| **Total**|                                                               |             |                                                   | **211,938,580** |

For more information visit [Silesia Corpus Homepage](https://sun.aei.polsl.pl/~sdeor/index.php?page=silesia).
