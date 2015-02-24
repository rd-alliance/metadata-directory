---
title: Worldwide Protein Data Bank Use Case
name: wwpdb-use-case
website: http://www.wwpdb.org
description: |
  Protein Data Bank archive (PDB) is the single worldwide archival repository of information about the 3D structures 
  of proteins, nucleic acids, and complex assemblies. The Worldwide PDB (wwPDB) organization manages the PDB archive 
  and ensures that the PDB is freely and publicly available to the global community.  The structure data in the PDB
  provides essential information for the understanding of biochemical processes and are critical data
  for structure-based drug design studies. These data are also central to the understanding the energetics
  of intermo- lecular interactions among proteins and nucleic acids, structure classification and structure prediction.
  The knowledge obtained through the study of 3D structure data is key to deducing the role of a protein or nucleic
  acid in human health and disease. 

  The PDB uses a community standard metadata representation, the Macromolecular Crystallographic Information Framework (mmCIF),
  orginally developed under the auspices of the International Union of Crystallography (IUCr). This representation
  extends the Crystallographic Information Framework (CIF) used by the IUCr as an electronic publication vehicle and by
  the Cambridge Crystallographic Data Center as an archiving standard.   The mmCIF standard was and subsequently
  extended by the wwPDB to include descriptions other experimental methods that produce 3D macromolecular structure
  models such as Nuclear Magnetic Resonance Spectroscopy, 3D Electron Microscopy and Tomography, and purely computational
  models.  Metadata extensions to support additonal experimental methods, hybrid and integrative methods are
  under development.

  The domain metadata for the PDB is currently managed in the PDB Exchange Data Dictionary (PDBx) which contains
  ~6600 data definitons.  Domain definitions are expressed using metadata framework containing
  ~150 attributes. The content of the PDBx dictionary evolves in response rapid developments methods and
  technologies in structural biology.  Content extensions of the PDBx dictionary are  managed by the wwPDB
  with input from community experts.  The PDBx dictionary is distributed in the in the original CIF syntax,
  in PDBML (XML/XSD), and RDF.

  The deposition and annotation software infrastructure developed by the wwPDB is built on the PDBx/mmCIF metadata
  framework.  The software tools leverage meta attributes describing boundary values, controlled vocabularies,
  data type, data patterns, and parent-child relationships to maintain data consistency.   Deposition and annotation
  user interfaces provide informative contextually relevant data descriptions taking advantage of semantic
  defintions and examples provided by the dictionary.    The PDBx/mmCIF data format is well
  supported by the most popular application packages that generate structure data for PDB deposition, and
  the format is also supported by popular bioinformatics and visualization tools. Tools are also available to build
  database schemas from the PDBx dictionary and to autogenerate loading tools for PDB structure entries. 

  Deposition of structure models and supporting experimental data are requirements for publication in the majority of
  scientific journals in which 3D structure models and experiments are reported.   The PDB also assigns DOIs
  to each of deposited data set.
 
subjects:
 - life-sciences
 - physical-sciences-and-mathematics
 - engineering
 - general
disciplines:
  # From HESA JACS Codes: http://www.hesa.ac.uk/content/view/1776/649/
 - biology
 - chemistry
 - physics
 - molecular-biology
 - structural-chemistry
 - biotechnology
 - bioinformatics
standards:
  # name of related standard
  - pdbx-mmcif
# The following are constants: do not modify
type: use_case
layout: use_case
---
