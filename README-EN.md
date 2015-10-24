# RegComplete
A private collection of frequently regular expression.

## Character

Contain uppercase/lowercase letters and half-size symbols.

CRLF & unlimited | CRLF & limited | no CRLF & unlimited| no CRLF & limited
------------ | ------------- | ------------ | -------------
^\D+$ | ^\D{`Min`, `Max`}$ | ^\D+ | ^\D{`Min`, `Max`} 

## Alphabet

Contain uppercase/lowercase letters, no half-size symbols.

CRLF & unlimited | CRLF & limited | no CRLF & unlimited| no CRLF & limited
------------ | ------------- | ------------ | -------------
^[a-zA-Z]+$ | ^[a-zA-Z]{`Min`, `Max`}$ | ^[a-zA-Z]+ | ^[a-zA-Z]{`Min`, `Max`} 

## Double Character

Contain Chinese and full-width symbols.

CRLF & unlimited | CRLF & limited | no CRLF & unlimited| no CRLF & limited
------------ | ------------- | ------------ | -------------
^[a-zA-Z]+$ | ^[a-zA-Z]{`Min`, `Max`}$ | ^[a-zA-Z]+ | ^[a-zA-Z]{`Min`, `Max`} 

## Numberic

Contain numbers.

CRLF & unlimited | CRLF & limited | no CRLF & unlimited| no CRLF & limited
------------ | ------------- | ------------ | -------------
^\d+$ | ^\d{`Min`, `Max`}$ | ^\d+ | ^\d{`Min`, `Max`} 

## Email

Email address.

CRLF & usual domain | no CRLF & usual domain | CRLF & unusual domain | no CRLF & unusual domain
------------ | ------------- | ------------ | -------------
^.+@.+\..{2,3}$ | ^.+@.+\..{2,3} | ^.+@.+\..+$ | ^.+@.+\..+

## IP

IPv4 address, contain `0.0.0.0` and `255.255.255.255`

((?:(?:25[0-5]|2[0-4]\d|((1\d{2})|([1-9]?\d)))\.){3}(?:25[0-5]|2[0-4]\d|((1\d{2})|([1-9]?\d))))$

## Username

Contain letters, numbers and underline, lenght limited.

^[a-zA-Z]\w{`Min`, `Max`}$

## Password

Must contain letters, numbers and symbols, lenght limited.

^(?!\D+$)(?![^a-zA-Z]+$)\S{`Min`, `Max`}$

## Cell Phone Number

Chinese cell phone number， contain country number.

^(0|86|17951)?(13[0-9]|15[012356789]|17[0678]|18[0-9]|14[57])[0-9]{8}$


