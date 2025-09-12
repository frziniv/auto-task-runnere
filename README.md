# auto-task-runnere
import os

print("System automation process initiated. Waiting for tasks...")
print("Performing system health check...")

# A simple check for disk space (example)
total, used, free = os.statvfs('/').f_frsize * os.statvfs('/').f_blocks, os.statvfs('/').f_frsize * (os.statvfs('/').f_blocks - os.statvfs('/').f_bfree), os.statvfs('/').f_frsize * os.statvfs('/').f_bavail
print(f"Disk Status: {free / (1024**3):.2f}GB free space available.")

print("Health check complete. System is ready.")
