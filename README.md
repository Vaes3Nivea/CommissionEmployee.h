# CommissionEmployee.h

//classe CommissiomEmployee
#ifndef COMMISSION_H
#define COMISSION_H

#include <string>
using std::string;

class CommissionEmployee
{
    public:
        CommissionEmployee( const string &, const string &, const string &, 
            double = 0.0, double = 0.0);

        void setFirstName(const string &);
        string getFirstName() const;

        void setLastName(const string &);
        string getLastName() const;

        void setSocialSecurityNumber(const string &);
        string getSocialSecurityNumber() const;

        void setGrossSales(const string &);
        string getGrossSales() const;

        void setCommissionRate(const string &);
        string getCommissionRate() const;

        double earsings() const;
        void print() const;
    private:
        string firstName;
        string lastName;
        string socialSecurityNumber;
        double grossSales;
        double commissionRate;

};

#endif
