# test
def main(txt):
    result = {}
    mass = txt.split(',')[:-1]
    for x in mass:
        val, per = x.split('>')
        val = val.split()[-2]
        val = int(val)
        per = per[1:-2].strip().strip('`')
        result[per] = val
    return result
