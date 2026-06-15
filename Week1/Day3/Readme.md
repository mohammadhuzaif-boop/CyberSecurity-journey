## Block 2 Theory: Linux Text Manipulation & Processes

### Text Manipulation Commands
- `cat` – prints file contents to the terminal
- `head -n <file>` – shows first n lines
- `tail -n <file>` – shows last n lines
- `grep "pattern" <file>` – searches for lines matching a pattern
- `wc -l` – counts lines
- `sort` – sorts lines alphabetically/numerically
- `uniq` – removes duplicate consecutive lines (often used with `sort`)
- Pipe `|` – sends output of one command as input to another

**Example:** Count how many lines in `access.log` contain "404"
```bash
grep " 404 " access.log | wc -l
**Process Management Commands**
ps aux – lists all running processes
top – real-time view of processes
kill <PID> – stops a process by its Process ID
sleep 300 & – runs a command in the background
Ctrl+Z – suspends the foreground process
fg – brings a background job to the foreground
bg – resumes a suspended job in the background
jobs – lists current background jobs

Example: Find and kill a process by name

bash
ps aux | grep nginx
kill <PID>
