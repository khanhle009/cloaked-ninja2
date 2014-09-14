#include <iostream>
#include <iomanip>
#include <math.h>

using namespace std;

int main()
{	
	double h;
	double v;
	int t;
	double g = 9.80;
	double pi = 3.14159265;

	cout << "Enter Initial Height:   ";
	cin >> h;

	cout << "Enter Initial Velocity: ";
	cin >> v;

	cout << "Enter Elapsed Time:     ";
	cin >> t;

	double heightAtTime = h + v * t - 1.0/2.0 * g * pow(t, 2.0);

	double groundTime = (2 * v) / g;

	cout << "The height at time " << t << " is " << fixed << setprecision(2) << heightAtTime << " meters.\n";

	cout << "At time " << fixed << setprecision(1) << groundTime << " seconds, the cannonball hits the ground.\n" << endl;

	cout << "The following table shows the range of the cannon for a ranges 25 to 60 in 5 degree increments.\n";

	cout << "     Angle          Range \n";

	int angle = 25;

	double s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);
	
	cout << fixed << setprecision(2) << "      " << angle << "           " << s << "\n";

	angle = 30;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 35;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 40;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 45;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 50;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 55;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	angle = 60;

	s = (2 * pow(v, 2) * cos ( angle * pi / 180.00 ) * sin ( angle * pi / 180.00 )) / (g);

	cout << "      " << angle << "           " << s << "\n";

	return 0;
}
