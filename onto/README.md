# File Format Ontology #

## Purpose of this document ##
This document documents the development of a file format ontology.

## Scope/Goal of the ontology ##
The ontology is developed to be used as common vocabularies to describe a file format. The document is expected to be in a binary format. The ontology only covers the interpretation of a byte string from a specific location in the file into a specified primitive datatype. The ontology does not cover how that piece of data is interpreted as the meaning of each terms is different based on the use of the file. 

## Roadmap ##
 1. Able to describe binary file format
 2. Able to describe text file format (config, ini, xml)
 3. Able to describe mixed-file format (text embedded in binary or binary embedded in text)

## Terms ##
 * File
 * BinaryFile
 * TextFile
 * Schema
 * Body
 * Bit
 * ByteString/Segment
 * Byte
 * Word
 * DoubleWord
 * QuadWord
 * Number
 * Integer
 * FloatingPoint
 * Character
 * FixedLength 
    (e.g. byte, word)
 * VariableLength 
    (e.g. string)
 * ComputedLength 
    (e.g. pascal string, palette)
 * MarkerTerminated 
    (e.g. null-terminated)
 
## Properties ##
 * bitLength (range: unsigned short integer)
 * hasExtension (range: string)
 * partOf/subsegmentOf

## Constraints ##
 - a file format can have more than 1 extension
 - a file extension can have more than 1 format (version)

## Inference Rules ##

## Sample Queries ##

## References ##
 * Sequence Ontology
 * Collection Ontology
 * Semantic XML