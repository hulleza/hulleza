from tkinter import*
import sqlite3

root=Tk()
root.title('Project 1')
root.geometry("500x500")
root.mainloop()
conn.commit()
conn.close()

f_name=Entry(root,width=30)
f_name.grid(row=0,column=1,padx=20)
l_name=Entry(root,width=30)
l_name(roow=1,colum=1,padx=20)
age=Entry(rot,width=30)
age.grid(row=2,column=1,padx=20)
address=Entry(root,width=30)
address.grid(row=3,column=1,padx=20)
email=Entry(root,width=30)
email.grid(row=4,column=1,padx=20)

f_name_label=Label(root,text="first Name")
f_name_label.grid(row=0,column=0)
l_name_label=Label(root,text="Last Name")
l_nanme_label.grid(row=1,column=0)
age_label_Label(root,text="age")
age_label.grid(row=2,column=0)
address_label_Lable(root,text="address")
address_label.grid(row=3,colum=0)
email_label_Label(root,text="email")
email_label.grid(row=4,column=0)

submit_btn=button(root,text="Add record to database",command=submit)
submit_btn.grid(row=6,column=0,columnspan=2,pady=0,padx=10,ipadx=100)

query_btn=button(root,text="show record",command=query)
query_btn.grid(row=7,column=0,columnspan=2,pady=10,padx=10,ipad=137

conn_sqlite3.connect('C:\Users\STUDENT8\AppData\Local\Programs\Python\Python312')
c=conn.consor()
c.execute("CREATE TABLE"myinfo"(
          "f_name"      TEXT,
          "l_name"      TEXT,
          "age"   INTEGER,
          "address"     TEXT,
          "email" TEXT

      )""")
""
def submit()

#database
conn=sqlite3.connect('C:/yser/CICT/data db')

#create cursor

c=conn.cursor()
#insert info Table

c.execute("INSERT INTO studentinfo
VALUES(f_name,l_name,age,address,email)",

     {
      'f_name':f_name.get()
      'l_name':l_name.get()
      'age':age.get()
      'address':address.get()
      'email':email.get()

      })
      #commitchanges
      conn.commit()

      #close connection
      conn.close()

      #clear the text boxe
      f_name delete(0,END)
      l_name delete(0,END)
      age delete(0,END)
      address delete(0,END)
      email delete(0,END)

          
           



