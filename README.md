# mousePosTest3
Mirror Reversal Precursor 3

Changes nessecary to get it to work

line 161, 238, 1374:
change the win references

i.e. win.mouseVisible = false ->
document.documentElement.style.cursor = 'none'

or

psychoJS.window.mouseVisible=true;

line 605, 606:
Change/add the appropriate JS math functions

i.e. pi -> Math.pi, sin -> Math.sin, cos -> Math.cos

line 678:
steps.append -> steps.push

line 819, 829:
change thisexp.addData to psychoJS.experiment.addData (this could be added to
the CurusorCode portion in psychopy builder.

Maybe changes:
const thisTrial = loop.getCurrentTrial();
        if (typeof thisTrial === 'undefined' || !('isTrials' in thisTrial) || thisTrial.isTrials) {
        
and change (trials) in routine statements to trials#

and maybe change 'trials.'
