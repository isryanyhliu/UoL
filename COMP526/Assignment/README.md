# COMP526 Assignment Folder

This folder contains assignments for **COMP526 - Applied Algorithmic Thinking**, part of the Advanced Computer Science MSc program at the University of Liverpool.

## Overview

The assignments in this folder focus on practical algorithm implementation and optimization problems, covering topics such as greedy algorithms, optimization strategies, and protocol design.

## Assignment Structure

### Assignment 01 - Bamboo Harvesting Optimization

**Location**: `01/`

**Problem Description**: 
A panda optimization problem involving bamboo harvesting strategies. The goal is to determine an optimal harvesting sequence that maximizes the guaranteed harvest from bamboo plots with different growth rates.

**Key Files**:
- `panda.py` - Core bamboo plot simulation framework
- `pandaYHCode.py` - Main solution implementation containing optimization algorithms
- `config.py` - Configuration file for student credentials
- `pandaYHCase.py` - Custom test case with growth rates `[10, 9, 6, 5, 4, 3, 2, 1, 1, 1]`

**Test Cases**:
- `pandaFibonacci.py` - Fibonacci sequence growth rates `[21, 13, 8, 5, 3, 2, 1, 1]`
- `pandaOdds.py` - Odd number sequence `[9, 7, 7, 5, 5, 3, 3]`
- `pandaMoreOdds.py` - Extended odd sequences
- `pandaOversupply.py` - Oversupply scenarios
- `pandaPower.py` - Power-based growth rates
- `pandaPrecision.py` - Precision-focused test cases
- `pandaUnequalPair.py` - Unequal pair scenarios

**Algorithm Features**:
- Greedy optimization for harvest timing
- Growth rate analysis and sorting
- Day-by-day simulation over 1,000,000 iterations
- Regular queue pattern detection for periodic harvesting

### Assignment 02 - Exam Cheating Protocol

**Location**: `02/`

**Problem Description**:
Implementation of a communication protocol for exam cheating scenarios, involving encoding and decoding strategies to transmit exam answers through limited communication channels.

**Key Files**:
- `examCheatingCode.py` - Main implementation with encoding/decoding functions
  - `compute_and_send_code(exam)` - Encodes 20-question exam into 10-bit code
  - `enter_solution_based_on_code(code)` - Decodes 10-bit code back to 20 answers
- `sitExam.py` - Exam simulation and testing framework

**Protocol Design**:
- **Encoding Strategy**: 
  - First 5 bits: Direct transmission of first 5 exam answers
  - Last 5 bits: Compressed representation of remaining 15 answers (3-to-1 compression)
  - Uses majority voting: groups of 3 answers compressed to 1 bit based on majority
- **Decoding Strategy**:
  - Direct extraction of first 5 answers
  - Expansion of compressed bits to triplets based on encoded values

## Technical Implementation

### Programming Language
- **Python 3.x** with standard libraries
- Uses collections, math, typing, json, itertools, and random modules

### Key Concepts Demonstrated

1. **Greedy Algorithms** (Assignment 01)
   - Optimal scheduling problems
   - Resource allocation strategies
   - Performance optimization over time

2. **Information Theory & Compression** (Assignment 02)
   - Data encoding/decoding protocols
   - Lossy compression strategies
   - Error analysis and worst-case scenarios

3. **Simulation & Testing**
   - Large-scale iterative simulation (1M+ iterations)
   - Comprehensive test case coverage
   - Performance measurement and validation

## Usage Instructions

### Assignment 01
1. Configure your username in `config.py`
2. Run specific test cases: `python pandaYHCase.py`
3. Results are saved to `{username}-results.json`

### Assignment 02
1. Test the protocol: `python sitExam.py`
2. Protocol handles all possible 2^20 exam combinations
3. Evaluates worst-case performance across all scenarios

## Files and Dependencies

### Generated Files
- `__pycache__/` - Python bytecode cache
- `psyli259-results.json` - Student results output

### Configuration
- Student MWS username required in `config.py`
- No external dependencies beyond Python standard library

---

*Part of COMP526 - Applied Algorithmic Thinking*  
*University of Liverpool - Advanced Computer Science MSc*