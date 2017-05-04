using System;
using System.Collections.Generic;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Linq;
using System.Text;
using System.Threading.Tasks;
using System.Windows.Forms;

namespace ChangeCalculator
{
    public partial class frmChangeCalculator : Form
    {
        public frmChangeCalculator()
        {
            InitializeComponent();
        }

        private void btnCalculate_Click(object sender, EventArgs e)
        {
            // get input from user for the amount of change
            int change = Convert.ToInt16(txtChange.Text);

            // initialize variables to be used in calculations
            int quarter = 25;
            int dime = 10;
            int nickel = 5;

            // calculate how many quarters
            int amount = change / quarter;

            // get remaining change after quarters
            change = change % quarter;

            // calculate how many dimes
            int amount1 = change / dime;

            // get remaining change after dimes
            change = change % dime;

            // calculate how many nickels
            int amount2 = change / nickel;

            // get amount of pennies by getting the remainder of the nickels
            int amount3 = change % nickel;

            // return the results to the textboxes
            txtQuarters.Text = amount.ToString();
            txtDimes.Text = amount1.ToString();
            txtNickels.Text = amount2.ToString();
            txtPennies.Text = amount3.ToString();

        }

        private void btnExit_Click(object sender, EventArgs e)
        {
            // close application
            this.Close();
        }
    }
}
