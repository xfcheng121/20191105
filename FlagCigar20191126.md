1.Explain BAM FLAG value：143

PAIRED,PROPER_PAIR,UNMAP,MUNMAP,READ2

该read是成对的paired reads中的一个
paired reads中每个都正确比对到参考序列上
该read没比对到参考序列上
与该read成对的matepair read没有比对到参考序列上
在paired reads中，该read是与参考序列比对的第二条
2.Explain BAM FLAG value： 99

PAIRED,PROPER_PAIR,MREVERSE,READ1

 该read是成对的paired reads中的一个
 paired reads中每个都正确比对到参考序列上
 与该read成对的matepair read其反向互补序列能够比对到参考序列
 在paired reads中，该read是与参考序列比对的第一条


3.Explain BAM FLAG value：516

 UNMAP,QCFAIL

 该read没比对到参考序列上
 该read没有通过质量控制

4.Explain BAM FLAG value： 2064

 REVERSE,SUPPLEMENTARY

 该read其反向互补序列能够比对到参考序列
 补充匹配的read

5.Explain BAM FLAG value： 147

 PAIRED,PROPER_PAIR,REVERSE,READ2

 该read是成对的paired reads中的一个
 paired reads中每个都正确比对到参考序列上
 该read其反向互补序列能够比对到参考序列
 在paired reads中，该read是与参考序列比对的第二条

6.Explain BAM CIGAR：14M2D31M

表示 reads 相对于第三列的 RNAME 序列，14 bp 能匹配上，随后有 2 bp 的删除，紧接着的 31 bp 能匹配上

7.Explain BAM CIGAR：3S6M1D5M

表示 reads 相对于第三列的 RNAME 序列，前 3 bp 不能匹配上，接着 6 bp 能匹配上，随后有 1 bp 的删除，之后的 5 bp 能匹配上

8.Explain BAM CIGAR: 6M14N5M

表示 reads 相对于第三列的 RNAME 序列，前 6 bp 能匹配上，接着跳过第三列的 RNAME 序列上 14 bp ，剩下的 5 bp 能匹配上

9.Explain BAM CIGAR: 7M5D8M2I14M  (小写：7m5d8m2i14m）

表示 reads 相对于第三列的 RNAME 序列，前 7 bp 能匹配上，接着有 5 bp 的删除，之后的 8 bp 能匹配上，随后发生了 2 bp 的插入，最后 14 bp 能匹配上

10.how long is the read with alignment CIGAR of 7M5D8M2I14M

31
