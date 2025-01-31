# Solutions Considered

1. **Loading Entire File in Memory (Rejected)**
   - Would cause memory overflow for a 1TB file.
   
2. **Streaming Approach (Chosen)**
   - Reads line by line, filtering only necessary data.
   - Efficient in time and memory.

# Final Solution Summary
- The script reads logs line by line and filters them based on the given date.
- It avoids memory issues by processing the file in chunks.
- Uses `startswith(date)` for fast filtering.
- Saves results directly to an output file.

# Steps to Run
1. Clone the repository:
   git clone https://github.com/ashutoash2908/tech-campus-recruitment-2025.git    

2. Run the script:
   python src/extract_logs.py  test_logs.log 2024-12-
01

3.  3. Output will be in `output/output_2024-12-01.txt`.
 