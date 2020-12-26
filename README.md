# List-of-semantically-linked-MWTs
A list of resources dedicated to semantic relation acquisition between multiwords terms or analogy test

## Context

The dataset is constructed as part of the Addicte project (Distributional analysis in specialized domain, ANR-17-CE23-0001), funded by the French National Research Agency (ANR). The dataset has been introduced in the paper "[A study of semantic projection from single word terms to multi-word terms in the environment domain](https://www.aclweb.org/anthology/2020.computerm-1.7/)", accepted by COMPUTERM 2020.

## Motivations

Current research on identifying relations between terms is mainly focused on single terms (SWT). However, MWTs and their semantically related terms are also in demand in many applications such as text simplification and machine translation, but only a few works concentrate on MWTs. We want to work on the semantic relation acquisition between MWTs and a list of semantically linked MWTs is then neccesary for our study. Since such a dataset does not yet exist in the domain that interests us (the environnemental domain), the first step of our work is to construct this dataset.

## Approche

The semantic projection also known as semantic variant and often referred to as a compositional method, is widely used to generate MWTs and predict relations between them from semantically related SWTs. This method is based on the assumption that MWT meaning is compositional. 

formally, let t1 and t2 be two MWTs such as $\text{\textbf{voc}}(t_1) = \{u_1, v_1\}$ and $\text{\textbf{voc}}(t_2) = \{u_2, v_2\}$ where $\text{\textbf{voc}}(x)$ is the set of the content words of $x$. If $u_1$ and $u_2$ are SWTs, if $v_1 = v_2$ and if there is a semantic relation $R$ between $u_1$ and $u_2$, then $R$ also holds between $t_1$ and $t_2$. In other words, if $\cal M$ is a set of MWTs of a domain and $\cal S$ is a set of SWTs, the hypothesis can be stated as follows:

<a href="https://www.codecogs.com/eqnedit.php?latex=\forall&space;t_1\in&space;{\cal&space;M},&space;\forall&space;t_2\in&space;{\cal&space;M}&space;\text{&space;such&space;as&space;}&space;\exists&space;u_1,&space;v_1,&space;u_2,&space;v_2&space;/\\&space;\text{\textbf{voc}}(t_1)&space;=&space;\{u_1,&space;v_1\}&space;\wedge&space;\text{\textbf{voc}}(t_2)&space;=&space;\{u_2,&space;v_2\}&space;\\&space;\wedge&space;u_1\in&space;{\cal&space;S}&space;\wedge&space;u_2\in&space;{\cal&space;S},\\&space;{[}&space;v_1&space;=&space;v2&space;\wedge&space;\exists&space;R,&space;R(u_1,&space;u_2)&space;\Rightarrow&space;R(t_1,&space;t_2)&space;{]}" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\forall&space;t_1\in&space;{\cal&space;M},&space;\forall&space;t_2\in&space;{\cal&space;M}&space;\text{&space;such&space;as&space;}&space;\exists&space;u_1,&space;v_1,&space;u_2,&space;v_2&space;/\\&space;\text{\textbf{voc}}(t_1)&space;=&space;\{u_1,&space;v_1\}&space;\wedge&space;\text{\textbf{voc}}(t_2)&space;=&space;\{u_2,&space;v_2\}&space;\\&space;\wedge&space;u_1\in&space;{\cal&space;S}&space;\wedge&space;u_2\in&space;{\cal&space;S},\\&space;{[}&space;v_1&space;=&space;v2&space;\wedge&space;\exists&space;R,&space;R(u_1,&space;u_2)&space;\Rightarrow&space;R(t_1,&space;t_2)&space;{]}" title="\forall t_1\in {\cal M}, \forall t_2\in {\cal M} \text{ such as } \exists u_1, v_1, u_2, v_2 /\\ \text{\textbf{voc}}(t_1) = \{u_1, v_1\} \wedge \text{\textbf{voc}}(t_2) = \{u_2, v_2\} \\ \wedge u_1\in {\cal S} \wedge u_2\in {\cal S},\\ {[} v_1 = v2 \wedge \exists R, R(u_1, u_2) \Rightarrow R(t_1, t_2) {]}" /></a>

For instance, the relation between the MWTs \emph{croissance de la population} `population growth' and \emph{diminution de la population} `population decline' is the same as the one between the SWTs \emph{croissance} `growth' and \emph{diminution}  `decline', that is antonymy. Our hypothesis is actually a bit stronger because we consider that the equivalence holds even when $t_1$ and $t_2$ do not have the same (syntactic) structure.
%

## Ressorces used for generating the dataset

## Different steps for generating the dataset

## Sample of the dataset
