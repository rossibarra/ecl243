## Count reads
1. Use `wc` to count the number of lines in file `F3D146_S212_L001_R2_001.fastq`. <br><br>
2. Use `grep` to count all the reads in file `F3D146_S212_L001_R2_001.fastq`. There are 4 lines for each read; does your answer match that from above? <br><br>
2. Write a script to use `grep` to make an output file with the read count in every fastq file in the directory. The file should have two tab-delimted columns with filename and read count in the two columns.

<details>
    <summary>HINTS</summary>

* Use `man` to get information on `wc` or to find out what `grep` flags to use.  

* See [here](http://maq.sourceforge.net/fastq.shtml) for information on fastq file format.  

* Using `^` to require a character to be at the beginning of a line or `$` to require something to be at the end of the line can help your `grep` query. For example `grep "A$"` only searches for lines that end with `A`.  

* Use `tr` to change one character into another. The tab character is `"\t"`.  

* You can pipe the output of one command into another using `|`. For example `echo "hello" | tr "h" "j"` should produce the output `"jello"`.
</p></details>
