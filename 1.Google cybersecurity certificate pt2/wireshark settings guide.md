
1. Change/manage profile
2. Auto adjust column widths to fit
3. refresh: runs file through rules again
4. Add filtering button: click -> add Label 
![[Pasted image 20240215085247.png|700]]

- Add packet diagram: Edit -> preferences -> appearance ->layout (select layout) (Pane:3 packet diagram (packet bytes can be useful for finding plaintext))
- Show packet diagram values:Right click packet diagram -> show field values
- Adding columns: Edit -> preferences -> appearance -> columns -> + (Title Delta, Type [[Delta time]] displayed)
- Add column: right click packet detail -> apply as column (e.g. [[TCP segment length]])
- Change Colouring rules :View-> colouring rules -> + (name: TCP SYN, Filter (tcp.flags.syn\==1, background, drag below Bad TCP))
- Filter without knowing command: Packet details -> right click a detail -> prepare as filter (selected), automatically inputs filter command
- Removing column header: right click column -> uncheck heading