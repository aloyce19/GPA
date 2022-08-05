class gpa:
    def __int__(self, subject, student):
        self.subject = subject
        self.student = student

    def result(self):
        x = int(input("Enter number of subject taken::: "))

        sub = []
        for i in range(x):
            subj_name = input("enter a subject name::")
            sub.append(subj_name)
        print(sub)

        dict = {}
        stdnm = []
        total = []
        y = int(input("Enter number of student::: "))
        for i in range(y):
            name_student = input("name of student:::")
            stdnm.append(name_student)

        print(stdnm)
        print("::ENTER A MARKS OF SUBJECT::")
        for i in stdnm:
            print(i)
            for x in sub:
                print(x)
                z = float(input("enter a marks:::"))
                marks = x + " = " + str(z)
                total.append(marks)
                # print(total)
                dict[i] = total
            print(dict)


p = gpa()

p.result()
