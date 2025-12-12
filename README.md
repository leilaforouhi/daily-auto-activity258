import datetime

def update_log():
    today = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
    
    with open("activity_log.txt", "a") as f:
        f.write(f"Activity recorded at: {today}\n")

    print(f"Daily activity saved: {today}")

if __name__ == "__main__":
    update_log()
