# Convert
进制间互相装换，
        System.out.println("Integer.parseInt");
        System.out.println(Integer.parseInt("17",16));//表示的是16进制的17，即16+7 =23,
        System.out.println( Integer.parseInt("17",10));//表示的是10进制的17，即10+7 =17
        System.out.println( Integer.parseInt("17",8));//表示的是8进制的17，即8+7 =15
        System.out.println( Integer.parseInt("17"));//不带参数，表示默认就是10进制的17，即17

        //public static Integer valueOf(String s, int radix)返回值是Integer型
        System.out.println("Integer.valueOf");
        System.out.println(Integer.valueOf("17",16));
        System.out.println(Integer.valueOf("17",10));
        System.out.println(Integer.valueOf("17",8));
        System.out.println(Integer.valueOf("17"));

        System.out.println("将10进制转换成其他进制:");
        System.out.println("10进制的10: "+Integer.toString(10));//10进制的10用2进制表示:10
        System.out.println("2进制的10: "+Integer.toBinaryString(10));//10进制的10用2进制表示：1010
        System.out.println("8进制的10: "+Integer.toOctalString(10));//10进制的10用8进制表示: 12
        System.out.println("16进制的10: "+Integer.toHexString(10));//10进制的10用16进制表示: a

        System.out.println("格式化转换10进制:");
        System.out.format("%d", 10).println();//结果为10
        System.out.format("%d", 010).println();//结果为8
        System.out.format("%d", 0x10).println();//结果为16

        System.out.println("格式化转换8进制:");
        System.out.format("%o", 10).println();//结果为12
        System.out.format("%o", 010).println();//结果为10
        System.out.format("%o", 0x10).println();//结果为20

        System.out.println("格式化转换16进制:");
        System.out.format("%x", 10).println();//结果为a
        System.out.format("%x", 010).println();//结果为8
        System.out.format("%x", 0x10).println();//结果为10

        System.out.println("格式化转换进制带#:");
        System.out.format("%#x", 10).println();//结果为0xa
        System.out.format("%#x", 010).println();//结果为0x8
        System.out.format("%#x", 0x10).println();//结果为0x10

        System.out.println("格式化转换进制带#:");
        System.out.format("%#4x", 10).println();//结果为0xa
        System.out.format("%#5x", 010).println();//结果为0x8
        System.out.format("%#6x", 0x10).println();//结果为0x10
