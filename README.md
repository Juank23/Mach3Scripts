# Mach3Scripts
Scripts for use with Mach3

<B><TT>AutoZero.m1s</TT></B> - A Mach3 Script to automatically find zero using a probe and a block with a hole that sits on the corner of the part. e.g. a modified <A HREF="https://triquetra-cnc.com/product/triquetra-p3-auto-zero-touch-plate-with-g-code-generator-copy/">Triquetra P3</A> with an optional hole drilled right over the part corner. <A HREF="https://www.youtube.com/watch?v=5V68e0A0uhQ">Example Video</A>. This is an update to the <A HREF="https://www.youtube.com/watch?v=XPNq4ys_Fjg">original code by Allan Massey</A> which adds support for using the hole to find the corner without entering the size of the bit. 

To install in Mach3 to go the Operator menu, Select "Edit button script" and then click the "Auto Tool Zero" button. Paste in this code, and save it. Before you exit Mach3, be sure to save configuration. 

To use, connect your probe and ground the bit, then place it on the corner of the part. Move the bit above the block for Z axis zero, to the side of the block toward the part on the X axis for outside zeroing (you will need to specify the size of the bit and it won't be exact), or move the bit inside the hole for completely automatic zeroing. Now push the "Auto Tool Zero" button. The status line will prompt you to touch the block to the bit to esure it is working within 15 seconds, then the selection dialog will show these options: <TT>Enter the Tool Diameter (in inches), or -2 to find in hole, or -1 to zero Z only</TT> The default is in hole as that doesn't need to know the bit size, and offers a more accurate zero in less time. 
