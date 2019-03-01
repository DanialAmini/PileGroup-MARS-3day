# PileGroup-MARS-3day
the multiple adaptive regression splines (MARS) method applied to pile group scour data for data having durations of 3days using package 'earth' in R software.<br />

The data are non-dimensionalized: <br />
inputs = `x1, x2, x3, x4`;
output = `z`

    x1=m
    x2=n
    x3=S'm/bp
    x4=S'n/bp
    z=be/(Ks*W)

`m`=number of piles inline with the flow <br />
`n`=number of piles perpendicular to the flow <br />
`bp`=pile diameter or width <br />
`Sm` & `Sn`=pile spacing inline and perpendicular with the flow <br />
`S'm=bp` if `m=1`, otherwise `S'm=Sm` <br />
`S'n=bp` if `n=1`, otherwise `S'n=Sn` <br />
`Ks`=shape factor=1.0 for group of cylinders, 1.1 for group of square piles <br />
`W=n*bp`=projected width of piles <br />
`be`=equivalent width of pile group, back-calculated from `y_s` (scour depth) values using FDOT-2010 equations <br />
