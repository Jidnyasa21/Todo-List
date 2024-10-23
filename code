class TodoList:
    def __init__(self):
        self.tasks = []

    def add_task(self, task):
        """Add a task to the to-do list."""
        self.tasks.append(task)
        print("Task added successfully!")

    def edit_task(self, index, new_task):
        """Edit a task at a specific index."""
        if 0 <= index < len(self.tasks):
            self.tasks[index] = new_task
            print("Task edited successfully!")
        else:
            print("Invalid task index")

    def delete_task(self, index):
        """Delete a task at a specific index."""
        if 0 <= index < len(self.tasks):
            del self.tasks[index]
            print("Task deleted successfully!")
        else:
            print("Invalid task index")

    def display_tasks(self):
        """Display the current list of tasks."""
        if self.tasks:
            print("Your To-Do List:")
            for i, task in enumerate(self.tasks, 1):
                print(f"{i}. {task}")
        else:
            print("Your To-Do List is empty!")

def main():
    todo_list = TodoList()
    while True:
        print("\n1. Add Task\n2. Edit Task\n3. Delete Task\n4. Display Tasks\n5. Exit")
        choice = input("Enter your choice: ")

        if choice == '1':
            task = input("Enter task: ")
            todo_list.add_task(task)
        elif choice == '2':
            index = int(input("Enter index of task to edit: ")) - 1
            new_task = input("Enter new task: ")
            todo_list.edit_task(index, new_task)
        elif choice == '3':
            index = int(input("Enter index of task to delete: ")) - 1
            todo_list.delete_task(index)
        elif choice == '4':
            todo_list.display_tasks()
        elif choice == '5':
            print("Exiting...")
            break
        else:
            print("Invalid choice. Please try again.")

if __name__ == "__main__":
    main()
