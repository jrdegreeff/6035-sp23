# 6.035 Computer Language Engineering SP23

__WE WILL MAKE ALL ANNOUNCEMENTS VIA [PIAZZA][piazza], SO MAKE SURE THAT YOU ENROLL__

If neither this site nor the Piazza has the information you need, you should [email the TA's directly](#course-staff)

## Table of Contents

1. [Schedule](#schedule-tentative)
1. [General Administrivia](#general-administrivia)
	1. [Course Staff](#course-staff)
	1. [MIT Catalog Description](#mit-catalog-description)
	1. [Recommended Texts](#recommended-texts)
	1. [Communication](#communication)
	1. [Grading](#grading)
	1. [Late policy](#late-policy)
	1. [Collaboration](#collaboration)
	1. [Compiler project](#compiler-project)
	1. [Class meetings](#class-meetings)
	1. [Contact](#contact)
	1. [Office Hours](#office-hours)
1. [Reference Materials](#reference-materials)
	1. [Official References](#official-references)
		1. [Provided During Exams](#provided-during-exams)
	1. [Unofficial References](#unofficial-references)

## Schedule (Tentative)

[Official MIT Calendar](https://registrar.mit.edu/calendar)

__!!! Note: This schedule is tentative and may change throughout the semester. !!!__


|                 | Monday                                | Tuesday                                 | Wednesday                                                                                | Thursday                                                          | Friday                                                                 |
|:---------------:|:-------------------------------------:|:---------------------------------------:|:----------------------------------------------------------------------------------------:|:-----------------------------------------------------------------:|:----------------------------------------------------------------------:|
| `02/06 - 02/10` | LOGISTICS FORM <br/> [L:intro][lec01] | [L: regular expressions][lec02]         | [L: regular expressions][lec02]                                                          | [L: grammars & parse trees][lec02]                                | [P1 RELEASE][P1 RELEASE]  <br/> [L: shift-reduce parsing][lec03]       |
| `02/13 - 02/17` | [L: shift-reduce parsing][lec03]      | [L: shift-reduce parsing][lec03]        | [L: shift-reduce parsing][lec03] <br/> [L: top-down parsing][lec04]                      | [L: top-down parsing][lec04]                                      | [L: top-down parsing][lec04]                                           |
| `02/20 - 02/24` | Presidents' Day Holiday               | [L: Intermediate Representation][lec05] | [L: Intermediate Representation][lec05]                                                  | [L:semantics][lec06]                                              | __P1 DUE @ 6:00PM__ <br/> [P2 RELEASE][P2 RELEASE]<br/>                |
| `02/27 - 03/03` | [L:codegen][lec07]                    | [L:codegen][lec07]                      | SUBMIT TEAM <br/>[L:codegen][lec07]                                                      | [L:codegen][lec07]                                                |                                                                        |
| `03/06 - 03/10` |                                       |                                         |                                                                                          |                                                                   | __P2 DUE @ 6:00PM__ <br/> [P3 RELEASE][P3 RELEASE] <br/> ADD DATE<br/> |
| `03/13 - 03/17` |                                       |                                         |                                                                                          |                                                                   | Quiz 1                                                                 |
| `03/20 - 03/24` | [L: program analysis 1][lec08]        | [L: program analysis 1][lec08]          | [L: program analysis 2][lec09]                                                           | [L: program analysis 2][lec09]                                    | [L: program analysis 2][lec09]                                         |
| `03/27 - 03/31` | Spring Break                          | Spring Break                            | Spring Break                                                                             | Spring Break                                                      | Spring Break                                                           |
| `04/03 - 04/07` | [L: loop optimization][lec10]         | [L: loop optimization][lec10]           | __P3 DUE @ 6:00PM__ <br/> [P4 RELEASE][P4 RELEASE] <br/> [L: register allocation][lec11] | [L: register allocation][lec11] <br/> [L: parallelization][lec12] | [L: parallelization][lec12]                                            |
| `04/10 - 04/14` | [L: dataflow][lec13]                  | [L: dataflow][lec13]                    | [L: dataflow][lec13]                                                                     | [L: dataflow][lec13]                                              | [L: dataflow][lec13]                                                   |
| `04/17 - 04/21` | Patriots' Day Holiday                 | [L: memory opt][lec14]                  | [L: memory opt][lec14]                                                                   |                                                                   | __P4 DUE @ 6:00PM__<br/>[P5 RELEASE][P5 RELEASE]<br/>                  |
| `04/24 - 04/28` |                                       | DROP DATE<br/>                          |                                                                                          |                                                                   | Quiz 2                                                                 |
| `05/01 - 05/05` |                                       | L: research                             | L: research                                                                              |                                                                   | __CHECKPOINT__                                                         |
| `05/08 - 05/12` |                                       |                                         |                                                                                          |                                                                   |                                                                        |
| `05/15 - 05/19` | __P5 DUE @ 11:59PM__                  | __LAST DAY__<br/>__L: DERBY__           |                                                                                          |                                                                   |                                                                        |


<!--- lecture slides --->
[lec01]: materials/lecture/lec01-Introduction.pdf
[lec02]: materials/lecture/lec02-RegularExpressionsAndGrammars.pdf
[lec03]: materials/lecture/lec03-shift-reduce-parsing.pdf
[lec04]: materials/lecture/lec04-top-down-parsing.pdf
[lec05]: materials/lecture/lec05-intermediate-representation.pdf
[lec06]: materials/lecture/lec06-semantic-analysis.pdf
[lec07]: materials/lecture/lec07-unoptimized-codegen.pdf
[lec08]: materials/lecture/lec08-program-analysis.pdf
[lec09]: materials/lecture/lec09-program-analysis-2.pdf
[lec10]: materials/lecture/lec10-loop-optimization.pdf
[lec11]: materials/lecture/lec11-register-allocation.pdf
[lec12]: materials/lecture/lec12-parallel.pdf
[lec13]: materials/lecture/lec13-foundations-of-dataflow.pdf
[lec14]: materials/lecture/lec14-memory_optimization.pdf

<!--- project phases --->
[P1 RELEASE]: phase-1/
[P2 RELEASE]: phase-2/
[P3 RELEASE]: phase-3/
[P4 RELEASE]: phase-4/
[P5 RELEASE]: phase-5/


<!--- others --->
[piazza]: https://piazza.com/mit/spring2023/6035


<!--- handouts --->
[project info]: materials/handouts/project-overview.pdf
[decaf spec]: materials/handouts/decaf-spec.pdf


## General Administrivia

### Course Staff

- Faculty
    - Martin Rinard <rinard@csail.mit.edu>

- TA
    - Alex Renda <renda@csail.mit.edu>
        - Office Hours: 36-144
            - Monday 5-6pm
            - Tuesday 6-7pm
    - Noah Raby <nbr@mit.edu>

### MIT Catalog Description

- Prereq -- `6.031`, `6.004`
- Level -- `U`
- Units -- `4-4-4`

Analyzes issues associated with the implementation of higher-level programming languages. Fundamental concepts, functions, and structures of compilers. The interaction of theory and practice. Using tools in building software. Includes a multi-person project on compiler design and implementation.

### Recommended Texts

6.035 has no officially required textbook. All of the material you need is taught in class, with the exception of the documentation for your implementation language and associated libraries. However, the following books may be helpful in implementing various components of your compiler, and are available from MIT libraries.

```txt
Modern Compiler Implementation in Java (Tiger Book)
Andrew W. Appel and Jens Palsberg
Cambridge University Press, 2002
```

Many other resources such as technical papers, interesting and useful blog posts, and reference guides are available on the references page.

### Communication

We will distribute assignments here and make all announcements via [Piazza][piazza]. Important announcements will also be made via email.

Since lecture dates are not all finalized at the start of the semester, please check the schedule regularly.

### Grading

| Component              | Weight |
|------------------------|--------|
| Project phases 2 and 3 | 25%    |
| Project phases 4 and 5 | 45%    |
| Quiz 1                 | 12%    |
| Quiz 2                 | 12%    |
| Miniquizzes            | 6%     |

For more information on the way the compiler project is graded, see the [project overview][project info].

### Late policy

We expect you to submit all components of the class on time. For extensions under extenuating circumstances (e.g., you are sick for a week, family emergencies), we require a letter from one of the student deans at S^3.

### Collaboration

Although you may discuss the projects with anybody, you must develop the code yourself. For the scanner/parser project, you must develop your code alone. On all subsequent projects, you should work with your team members, but you may not develop or share any code with other teams.

You may collaborate on the mini-quizzes and the problem sets, but you should write all solutions yourself.

Do not post your lab or homework solutions on publicly accessible web sites or file spaces; this enables cheating for students in future years.

### LLM policy

ChatGPT/Copilot/other LLMs are capable of generating code examples for many of the tasks you will complete. It's OK to take a look at these code examples. It is not OK to substantially use this generated code directly in your project.

### Compiler project

This class involves a group project, where you will build a compiler almost entirely from scratch. Details about the project can be found [here][project info]. Specific instructions for each phase of the project will be released later in the class.

### Class meetings

Lectures:

- 11am-12pm MTWRF in [32-124](http://whereis.mit.edu/?mapterms=32).

### Contact

For all general questions and/or concerns, please post on Piazza.

If the matter is private, please email the TA's directly.

### Office Hours

Refer to Piazza for the latest updates about office hours. We will have additional office hours before each quiz and each phase of the project.

## Reference Materials

This section contains a number of useful and/or interesting references selected by the staff. You are not expected to know most of the material on this page for the class; however, you may find it interesting and helpful.

### Official References

1. The complete [Intel x64 manual](http://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-software-developer-manual-325462.pdf)
1. [Intel x64 Optimization Reference Manual](http://www.intel.com/content/dam/www/public/us/en/documents/manuals/64-ia-32-architectures-optimization-manual.pdf)
1. [x64 wiki](https://en.wikibooks.org/wiki/X86_Assembly/X86_Instructions)
1. [x64 cheat sheet](https://cs.brown.edu/courses/cs033/docs/guides/x64_cheatsheet.pdf) -- lists and tables detailing registers and assembly commands
1. [x86-64 architecture guide](http://6.035.scripts.mit.edu/fa18/x86-64-architecture-guide.html) -- a walkthrough with an example, and common commands
1. [Intel x64 manual](https://software.intel.com/en-us/articles/intel-sdm)
1. [Intel developer manual](https://software.intel.com/sites/default/files/managed/39/c5/325462-sdm-vol-1-2abcd-3abcd.pdf) -- detailed description of some assembly instructions

#### Provided During Exams

1. [x64 cheat sheet](https://cs.brown.edu/courses/cs033/docs/guides/x64_cheatsheet.pdf) -- lists and tables detailing registers and assembly commands

### Unofficial References

Interesting blog posts, papers, etc

1. Overviews
    1. [LLVM compiler architecture](http://www.aosabook.org/en/llvm.html)
    1. [GCC compiler architecture](http://en.wikibooks.org/wiki/GNU_C_Compiler_Internals/GNU_C_Compiler_Architecture)
1. Blogs
    1. [Russ Cox's Blog](http://research.swtch.com/) -- Russ is one of the developers of Google Go, a pretty interesting language.
    1. [Ian Wienand's Blog](http://www.technovelty.org/) -- Whoever he is, he writes about compiler and language internals, the magic black box that is the linker, and more
    1. [Matt Might's Blog](http://matt.might.net/articles/) -- Matt is a professor at the University of Utah and has written some very interesting articles (e.g. "Yacc is dead")
1. Papers
    1. [Register Allocation & Spilling via Graph Coloring](http://dl.acm.org/citation.cfm?id=806984) -- G.J. Chaitin / 1982. Great (short) paper on simple register allocation.
    1. [Linear Scan Register Allocation](https://dl.acm.org/citation.cfm?id=330250)
    1. [Iterated Register Coalescing](http://dl.acm.org/citation.cfm?id=229546) -- Lal George / 1996. Presents improvements/alternative to Chaitin's design. If Chaitin-style (+/-Briggs) register allocation isn't enough for you, this paper is a good read - actually, it's a good read anyway, to understand the tradeoffs
    1. [Superword Level Parallelism](http://dl.acm.org/citation.cfm?id=358438) combined with loop unrolling, a simple way to implement a vectorizing compiler
1. Miscellaneous
    1. [Scala Patterns for Compiler Design](https://gist.github.com/rcoh/4992969)
    1. `6.823 Advanced Computer Architecture` [lecture notes](http://csg.csail.mit.edu/6.823/lecnotes.html)
    1. [The Missing Semester of Your CS Education](https://missing.csail.mit.edu/2020/)
