# Comparison with State-of-the-art Approaches

## Tables show the deobfuscation results of DiANa.  
(R2) Red part is the results of [35]'s unflow-sensitive approach. Notice that samples in Table.2 and 3 are all in-the-wild O-LLVM obfuscated apps, and DiANa works on function level. DiANa is evaluated on 65 functions with in-the-wild obfuscation.

![avatar](result/1.png)
![avatar](result/2.png)

It can be seem that our results are significantly better than [35] on all three benchmarks because of the Flow-Sensitive deobfuscation, especially on large functions (i.e., romannumerals, reverse, CVE-functions) and enhanced O-LLVM obfuscation (CFF-3 and ALL). On the first and third benchmark we used, [35] could only achieve ~40% of CFG similarity after deobfuscation, while DiANa could achieve 83% on average. This comparison will be updated in the revision.

## (R1/R2) Also, we use a high-level algorithm to re-describe the workflow.

![avatar](algorithm/chopped_symbolic_execution.png)

