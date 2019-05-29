# Assignment-STM
STM Assignment
Containing Rectangle Class
..........................
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace Assignment1
{
    public class Rectangleclass
    {
        private int length1;
        private int width1;

        public Rectangleclass()
        {
            length1 = 1;
            width1 = 1;
        }

        public Rectangleclass(int length1, int width1)
        {
            this.length1 = length1;
            this.width1 = width1;
        }

        public int GetLength()
        {
            return length1;
        }
        public int SetLength(int length1)
        {
            this.length1 = length1;
            return this.length1;
        }

        public int GetWidth()
        {
            return width1;
        }

        public int SetWidth(int width1)
        {
            this.width1 = width1;
            return this.width1;
        }

        public int GetPerimeter()
        { 
            return 2*(length1 + width1);
        }

        public int GetArea()
        {
            return (length1 * width1);
        }
    }
}
