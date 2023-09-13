# Project_
наработка

double.TryParse(textBox1.Text, out x) && double.TryParse(textBox2.Text, out y) &&
                double.TryParse(textBox3.Text, out z))
            {
                
         double res = (Math.Pow((8 + Math.Pow(Math.Abs(x - y), 2) + 1),1 / 3) /
          ((Math.Pow(x, 2) + Math.Pow(y, 2) + 2))) - Math.Exp(Math.Abs(x - y)) *
                Math.Pow((Math.Pow(Math.Tan(z), 2) + 1), x);
                textBox4.Text += Environment.NewLine+"Лаб.раб.№1 Бондарь Ю.В. гр.10701222" + Environment.NewLine + "Х =" + x.ToString() + Environment.NewLine + "Y =" + y.ToString() +
                Environment.NewLine + "Z =" + z.ToString() + Environment.NewLine + "Резульат:" +
                res.ToString() + Environment.NewLine;
                
            }
            else
            {
                MessageBox.Show("Введенные данные не являются числом, введите числовые данные!");
            }
        }
    }
}
