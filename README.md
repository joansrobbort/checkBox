    @IBOutlet weak var btn5: UIButton!
    @IBOutlet weak var btn7: UIButton!
    @IBOutlet weak var btn6: UIButton!




@IBAction func TapToCheck(_ sender: UIButton) {
        if sender == self.btn5 {
            self.btn5.isSelected = !btn5.isSelected
            
            if btn5.isSelected{
                ArraySelected.append("5")
            }else{
               let str5 = ArraySelected.index(of: "5")
                ArraySelected.remove(at: str5!)
            }
        }
        else if sender == self.btn6 {
             self.btn6.isSelected = !btn6.isSelected
            if btn5.isSelected{
                ArraySelected.append("6")
            }else{
                let str6 = ArraySelected.index(of: "6")
                ArraySelected.remove(at: str6!)
            }
            
        }else{
             self.btn7.isSelected = !btn7.isSelected
            if btn5.isSelected{
                ArraySelected.append("7")
            }else{
                let str7 = ArraySelected.index(of: "7")
                ArraySelected.remove(at: str7!)
            }
            
        }
    }
