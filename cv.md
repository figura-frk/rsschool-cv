# **Anna Figura**
###### anna.figura259@gmail.com | [[Website](afigura.com) | [Telegram](https://t.me/figura_frk)
___
### Summary
> Hello, my name is Anna and my passion always were people and design. I met so many
and great people in Accenture, so I can be proud that I have such an amazing team,
they are taking my heart. I can’t live without design so it’s my soul and my mind.
Working as a freelance UX/UI Web designer I am gaining new experiences, emotions and
inspiration every time. If you are a designer - you will never stop improving. Recently
I've started my learning journey with RS school, learning JS.

### Skills

- Github
- Visual Studio
- Android Studio
- Pycharm
- Adobe Kit
- Google Office Kit

### Latest Code Example

``` package ua.primer

import android.os.Bundle
import android.widget.CheckBox
import androidx.appcompat.app.AppCompatActivity
import kotlinx.android.synthetic.main.activity_main.*

class MainActivity : AppCompatActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        cbAll.setOnCheckedChangeListener { _, isChecked ->
            onAllCheckBoxStateChanged(isChecked)
        }
        cbFirst.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbSecond.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbThird.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbFirstCopy.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbSecondCopy.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbThirdCopy.setOnCheckedChangeListener { _, _ -> verifyAllCheckBoxes() }
        cbAllCopy.setOnCheckedChangeListener { _, isChecked ->
            onAllCheckBoxStateChangedCopy(
                isChecked
            )
        }
    }

    private fun onAllCheckBoxStateChanged(flag: Boolean) = if (flag) {
        cbFirst.isChecked = true
        cbSecond.isChecked = true
        cbThird.isChecked = true

    } else {
        cbFirst.isChecked = false
        cbSecond.isChecked = false
        cbThird.isChecked = false
    }

    private fun onAllCheckBoxStateChangedCopy(flag: Boolean) = if (flag) {
        cbFirstCopy.isChecked = true
        cbSecondCopy.isChecked = true
        cbThirdCopy.isChecked = true
    } else {
        cbFirstCopy.isChecked = false
        cbSecondCopy.isChecked = false
        cbThirdCopy.isChecked = false
    }

    private fun verifyAllCheckBoxes() {
        val checkBoxStateList = listOf(
            cbFirst.isChecked,
            cbSecond.isChecked,
            cbThird.isChecked
        )
        val checkBoxStateListCopy = listOf(
            cbFirstCopy.isChecked,
            cbSecondCopy.isChecked,
            cbThirdCopy.isChecked
        )

        val obligatoryList = listOf(
            cbFirst.isChecked,
            cbSecond.isChecked,
            cbFirstCopy.isChecked,
            cbSecondCopy.isChecked
        )

        btResult.isEnabled = !obligatoryList.any { !it }

        toggleAllCheckboxState(!checkBoxStateList.any { !it })
        toggleAllCheckboxStateCopy(!checkBoxStateListCopy.any { !it })
    }

    private fun toggleAllCheckboxState(state: Boolean) {
        cbAll.setOnCheckedChangeListener(null)
        cbAll.isChecked = state
        cbAll.setOnCheckedChangeListener { _, isChecked ->
            onAllCheckBoxStateChanged(isChecked)
        }
    }

    private fun toggleAllCheckboxStateCopy(state: Boolean) {
        cbAllCopy.setOnCheckedChangeListener(null)
        cbAllCopy.isChecked = state
        cbAllCopy.setOnCheckedChangeListener { _, isChecked ->
            onAllCheckBoxStateChangedCopy(isChecked)
        }
    }

}
```
### Experience
**Jr. Team Leader at Accenture Operations, Cracow**
_February 2020 - Present_

**Junior Designer (Part time) at Digishares, Copenhagen**
_November 2019 - Present_

**Junior Designer at Freelance Marketing Services**
_January 2020 - May 2020_

**Quality Analyst at Accenture Operations, Cracow**
_September 2018 – January 2020_

**Junior Web Data Analyst at Accenture Operations, Cracow**
_December 2017 – August 2018_