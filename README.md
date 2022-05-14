# Vector-vs-ArrayList-in-Java convert vector to arraylist in java
Vector vs ArrayList in Java convert vector to arraylist in java

Convert Vector to ArrayList in Java There are multiple ways to convert vector to ArrayList, using passing the Vector in ArrayList constructor and by using simple vector traversal and adding values to ArrayList.

What is difference between Vector class and ArrayList class?

Vector is similar to ArrayList but the differences are, it is synchronized and its default initial size is 10 and when the size exceeds its size increases to double of the original size that means the new size will be 20. Vector is the only class other than ArrayList to implement RandomAccess.

 
 DefaultTableModel dt = (DefaultTableModel) jTable1.getModel();
        
        Vector v = new Vector();
        v.add(Name);
        v.add(Qty);
        v.add(d11);
        dt.addRow(v);

// First way	
ArrayList<String> Arrlist = new ArrayList<String>();  
        // Convert Vector to ArrayList
        for (int i = 0; i < v.size(); i++)
            Arrlist.add(v.get(i));
        // add ArrayList DefaultTableModel
        dt.addRow(Arrlist);

//secong way :
		// Convert Vector to ArrayList
        ArrayList<String> Arrlist= new ArrayList<String>(v);
  
       // add ArrayList DefaultTableModel
        dt.addRow(Arrlist);
