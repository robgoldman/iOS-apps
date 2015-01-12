//
//  ViewController.swift
//  Tips Demo for Entry to Class
//
//  Created by Robert Goldman on 1/11/15.
//  Copyright (c) 2015 Robert Goldman. All rights reserved.
//

import UIKit

class ViewController: UIViewController {
    @IBOutlet weak var billField: UITextField!
    @IBOutlet weak var tipLabel: UILabel!
    @IBOutlet weak var tipControl: UISegmentedControl!
    @IBOutlet weak var totalLabel: UILabel!
    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
    
   
    

    tipLabel.text = "$0.00"
    totalLabel.text = "$0.00"
    }
    
    override func didReceiveMemoryWarning() {
        super.didReceiveMemoryWarning()
        // Dispose of any resources that can be recreated.
    }

    @IBAction func onEditingChanged(sender: AnyObject) {
    
        var tipPercentages=[0.15, 0.20, 0.25]
        var tipPercentage = tipPercentages[tipControl.selectedSegmentIndex]
        var billAmount = (billField.text as NSString).doubleValue
        var tip = billAmount * tipPercentage
        var total = billAmount + tip
        tipLabel.text = "$\(tip)"
        totalLabel.text = "$\(total)"
        tipLabel.text = String(format: "$%.2f", tip)
        totalLabel.text = String(format: "$%.2f", total)
        println(total)
        
        
    }

    
    
   
    
    @IBAction func onTap(sender: AnyObject) {view.endEditing(true)
    }
    
    
}
