# Assignment-STM
STM Assignment
Containing Unit tests
..........................
using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using Assignment1;
using NUnit.Framework;

namespace Assignment_tests
{
    [TestFixture]
    class Assignment_tests
    {
        [Test]
        public void GetRectangleLength_InputLength10_expectedResultEquals10()
        {
            //Arrange
            int l1 = 10;
            int w1 = 8;
            int expectedoutput = l1;
            Rectangleclass testres = new Rectangleclass(l1, w1);

            //Act
            int actualoutput = testres.GetLength();

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
        [Test]
        public void SetRectangleLength_InputLength33_expectedResultEquals33()
        {
            //Arrange
            int l1 = 33;
            int w1 = 18;
            int expectedoutput = l1;
            Rectangleclass testres = new Rectangleclass(l1,w1);

            //Act
            int actualoutput = testres.SetLength(l1);

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
        [Test]
        public void GetRetangleWidth_InputWidth199_expectedResultEquals199()
        {
            //Arrange
            int l1 = 19;
            int w1= 199;
            int expectedoutput = w1;
            Rectangleclass testres = new Rectangleclass(l1, w1);

            //Act
            int actualoutput = testres.GetWidth();

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
        [Test]
        public void SetRectangleWidth_InputWidth26_expectedResultEquals26()
        {
            //Arrange
            int l1 = 10;
            int w1 = 26;
            int expectedoutput=w1;
            Rectangleclass testres = new Rectangleclass(l1, w1);

            //Act
            int actualoutput = testres.SetWidth(w1);

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
        [Test]
        public void GetRectanglrPerimeter_Length10Width20_expectedResultEquals60()
        {
            //Arrange
            int l1 = 10;
            int w1 = 20;
            int p = 2 * (l1 + w1);
            int expectedoutput = p;
            Rectangleclass testres = new Rectangleclass(l1, w1);

            //Act
            int actualoutput = testres.GetPerimeter();

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
        [Test]
        public void GetRectangleArea_Length12Width11_expectedResultEquals132()
        {
            //Arrange
            int l1 = 12;
            int w1 = 10;
            int a = (l1 * w1);
            int expectedoutput = a;
            Rectangleclass testres = new Rectangleclass(l1, w1);

            //Act
            int actualoutput = testres.GetArea();

            //Assert
            Assert.AreEqual(expectedoutput, actualoutput);
        }
    }
}
