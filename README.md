BCD_7SEGMENT

![image](https://github.com/priyangi123/priyangi123/assets/165141104/982c3b13-792c-4b50-939f-86695185563e)

# VERILOG CODE:

module segment7(

 bcd,

 seg

);

 input [3:0] bcd;

 output [6:0] seg;
 
 reg [6:0] seg;

always @(bcd)

begin

    case (bcd)
    
        0 : seg = 7'b0000001;
        
        1 : seg = 7'b1001111;
        
        2 : seg = 7'b0010010;
        
        3 : seg = 7'b0000110;
        
        4 : seg = 7'b1001100;
        
        5 : seg = 7'b0100100;
        
        6 : seg = 7'b0100000;
        
        7 : seg = 7'b0001111;
        
        8 : seg = 7'b0000000;
        
        9 : seg = 7'b0000100;
        
        default : seg = 7'b1111111; 
    
    endcase

end

endmodule


# OUTPUT:


![image](https://github.com/priyangi123/priyangi123/assets/165141104/4cb98f8a-e281-4507-a4fd-4d10864a4cd4)
