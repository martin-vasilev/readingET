
Meaning of the data output columns:

- **sub**: subject.
- **item**: experimental item.
- **cond**: condition number. Taken from data file (if avalable). Otherwise it's NA.
- **seq**: trial sequence. This shows the trial history (e.g., seq 1 appeared as first trial, seq 2 as second trial and so on).
- **SFIX**: start of fixation flag (in asc. file). This can be used to search in the raw data to easily locate the fixation.
- **EFIX**: end of fixation flag (see above).
- **xPos**: x position of the fixation on the screen (in pixels).
- **yPos**: y position of the fixation on the screen (in pixels).
- **fix_num**: (serial) number of the fixation in the trial (e.g., 1 was the first first fixation in this trial, 2 was the second fixation and so on).
- **fix_dur**: duration of the fixation (in ms). This is calculated by substracting the SFIX flag from the EFIX flag.
- **sacc_dur**: duration of the saccade immediately prior to this fixation (in ms).
- **sent**: Sentence number of the text where the fixation occured. This has been tested only in English; please exert caution with other languages.
-  **line**: Line of text on which the fixation occured.
- **word**: Word number on which the fixation occurred. This has been tested only in English. Inaccuracies are possible if there are unusual symbols in the text.
- **char_trial**: character number on in the trial on which the fixation occured (this includes all text presented in the trial).
- **char_line**: character number on the line where the fixation occured (this counts only the characters that were on a given line of text).
- **regress**: a logical indicating whether the current fixation was a regressive one (1= yes; 0= no).
- **wordID**: a letter string of the word that was fixated during this fixation.
- **land_pos**: landing posisition (in characters) on the word. 0 means that the empty space before the word was fixated.
- **sacc_len**: length of the incoming saccade (in characters).
- **blink**: a logical indicating whether there was a blink during the fixation (1= yes; 0= no).
- **prev_blink**: a logical indicating whether there was a blink x ms before the start of the fixation (x is user-defined; default is 50ms) (1= yes; 0= no).
- **next_blink**: a logical indicating whether there was a blink x ms after the end of the fixation (x is user-defined; default is 50ms) (1= yes; 0= no).
- **outOfBnds**: a logical indicating whether the fixation occured out of bounds (i.e., outside the screen area) (1= yes; 0= no). This can happen due to blinks/ track losses, if participant moves their head, etc.
- **outsideText**: a logical indicating whether the fixation occured outside the text area on the screen (1= yes; 0= no).
- **hasText**: a logical indicating whether text was displayed on the trial (1= yes; 0= no).
0 can occur if the text was presented as images or was not otherwise printed to the asc. file.
- **dataFile**: name of the data file from which the fixation was extracted.